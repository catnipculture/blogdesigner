> #### 作者主页：[舒克日记](https://blog.csdn.net/cativen)
>
>  简介：Java领域优质创作者、Java项目、学习资料、技术互助
>
> <b><font color=red>文中获取源码</font></b>

# 项目介绍

论坛系统设置的角色有管理员，版主，用户等。



管理员管理论坛，主要是对论坛帖子增删改查以及对论坛帖子回复进行查看，对版主和用户进行管理，管理新闻等。



版主可以发布帖子，可以查询论坛帖子，可以对论坛帖子回复进行查看，可以回复帖子，可以删除帖子，可以查看新闻，更改个人信息等。



用户在前台查看新闻，在留言版对发布的留言和管理员的回复进行查看，在论坛模块发帖，评论帖子，查看帖子。



# 环境要求



1.运行环境：最好是java jdk1.8,我们在这个平台上运行的。其他版本理论上也可以。 

2.IDE环境：IDEA,Eclipse,Myeclipse都可以。推荐IDEA; 

3.tomcat环境：Tomcat7.x,8.X,9.x版本均可 

4.硬件环境：windows7/8/10 4G内存以上；或者Mac OS; 

5.是否Maven项目：是；查看源码目录中是否包含pom.xml;若包含，则为maven项目，否则为非maven.项目 

6.数据库：MySql5.7/8.0等版本均可；





# 技术栈



运行环境：jdk8 + tomcat9 + mysql5.7 + windows10

服务端技术：SpringBoot + MyBatis + Vue + Bootstrap + jQuery





# 使用说明





1.使用Navicat或者其它工具，在mysql中创建对应sq文件名称的数据库，并导入项目的sql文件； 

2.使用IDEA/Eclipse/MyEclipse导入项目，修改配置，运行项目； 

3.将项目中config-propertiesi配置文件中的数据库配置改为自己的配置，然后运行；





# 运行指导

idea导入源码空间站顶目教程说明(Vindows版)-ssm篇：

http://mtw.so/5MHvZq 

源码地址：[http://www.codegym.top](http://www.codegym.top/)




# 运行截图

![img](https://img-blog.csdnimg.cn/img_convert/9050fc922cb5a89ea2670cd9119580a1.png)



![img](https://img-blog.csdnimg.cn/img_convert/2393bf86a6e7a09215367b8941294f21.png)



![img](https://img-blog.csdnimg.cn/img_convert/7e7f3b6020bb69fcae7404d5dbc5ddb6.png)

### 前台

![springboot201基于SpringBoot的论坛系统设计与实现6](https://img-blog.csdnimg.cn/img_convert/dd46d623be376a171f9b95f666ee747c.png)

![springboot201基于SpringBoot的论坛系统设计与实现7](https://img-blog.csdnimg.cn/img_convert/d9d9e219998ebeabfd71848dabd2c5a3.png)

![springboot201基于SpringBoot的论坛系统设计与实现8](https://img-blog.csdnimg.cn/img_convert/cab42e71ec39859d01de7f19ed04f873.png)



### 后台

![springboot201基于SpringBoot的论坛系统设计与实现0](https://img-blog.csdnimg.cn/img_convert/15282b047de7d302e2839f061aee1d3f.png)

![springboot201基于SpringBoot的论坛系统设计与实现1](https://img-blog.csdnimg.cn/img_convert/78615595432e22ee67ee05f615a18ccf.png)

![springboot201基于SpringBoot的论坛系统设计与实现2](https://img-blog.csdnimg.cn/img_convert/16a73a268899ddd88322d897cb662d84.png)

![springboot201基于SpringBoot的论坛系统设计与实现3](https://img-blog.csdnimg.cn/img_convert/cb0e717f4c1abc2ce4fd4c8f7f9098b0.png)

![springboot201基于SpringBoot的论坛系统设计与实现4](https://img-blog.csdnimg.cn/img_convert/77be67e8049f155d073a714bd3696216.png)

![springboot201基于SpringBoot的论坛系统设计与实现5](https://img-blog.csdnimg.cn/img_convert/b81bf4b7019267e43e70a6d378f0b722.png)

### 代码



```java
public interface CaipinxinxiService extends IService<CaipinxinxiEntity> {

    PageUtils queryPage(Map<String, Object> params);
    
   	List<CaipinxinxiVO> selectListVO(Wrapper<CaipinxinxiEntity> wrapper);
   	
   	CaipinxinxiVO selectVO(@Param("ew") Wrapper<CaipinxinxiEntity> wrapper);
   	
   	List<CaipinxinxiView> selectListView(Wrapper<CaipinxinxiEntity> wrapper);
   	
   	CaipinxinxiView selectView(@Param("ew") Wrapper<CaipinxinxiEntity> wrapper);
   	
   	PageUtils queryPage(Map<String, Object> params,Wrapper<CaipinxinxiEntity> wrapper);
   	
}


```


