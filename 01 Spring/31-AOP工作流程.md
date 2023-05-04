# 31-AOP工作流程

AOP 的工作模式：代理模式

![](../img/20230503080454.png)

一旦 bean 有使用到切入點，那麼該 bean 就會被生成成Proxy物件

- 如果直接去印有被代理的 bean ，他一樣會印原本物件的reference，因為該 proxy 物件的 toString方法已被Override
- 如果印的是 bean.getClass() 那麼就可以實質看到該物件為 Proxy 物件！

![](../img/20230503081207.png)
![](../img/20230503081213.png)

