
<font color=#999AAA >############################

</font>

@[TOC](UML图详细图文教程)


<hr style=" border:solid; width:100px; height:1px;" color=#000000 size=1">
<font color=#999AAA >###############################

</font>

# 前言

<font color=#999AAA >
刚刚参加工作，领导让我认识软件结构，熟悉每个模块的调用过程，简直裂开（@-@），不要说每个模块都有上百个方法，就是他们调来调去的关系，我就画了一整张纸，密密麻麻，睡醒觉第二天就已经看不懂了，前辈说”工具不对“
才接触到UML，刚开始也是一头雾水，通过学习一段时间，把我的成果和感受，和大家分享，欢迎指正！
</font>

<hr style=" border:solid; width:100px; height:1px;" color=#000000 size=1">

<font color=#999AAA >

# 一、UML图是什么？


<font color=#999AAA >
UML-Unified Modeling Language 统一建模语言，又称标准建模语言。是用来对软件密集系统进行可视化建模的一种语言。UML的定义包括UML语义和UML表示法两个元素。
UML是在开发阶段，说明、可视化、构建和书写一个面向对象软件密集系统的制品的开放方法。最佳的应用是工程实践，对大规模，复杂系统进行建模方面，特别是在软件架构层次，已经被验证有效。统一建模语言（UML）是一种模型化语言。模型大多以图表的方式表现出来。一份典型的建模图表通常包含几个块或框，连接线和作为模型附加信息之用的文本。这些虽简单却非常重要，在UML规则中相互联系和扩展。</font>

##实在是不好意思以上都是百度复制下来的。。。##
以我的理解来看，标准化建模语言，更加贴近真实的代码结构，逻辑更加清晰，把复杂的的模块逻辑调用细分，这大概就是他存在的意义。



# 二、认识组件
以Enterprise Architect为例
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202135711243.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)

## 1.需求视图
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202140223214.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)![在这里插入图片描述](https://img-blog.csdnimg.cn/202102021403099.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
例如UML图中的项目文件结构应和真正的项目结构一致，这样就一目了然
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202140643662.png)
点击在model中新建new Package（可以和项目中的工程文件同名，便于阅读）
==模块总目录>单个模块文件>需求视图&逻辑视图==
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202140946857.png)
 如此我们便得到了一个模块；
那么现在我们要开始着手画UML图了；
和软件开发一样，我们首先要对模块做系统的需求分析（在实际开发中每个需求都会有和他相对应的方法，这也是我们后面要用到的，所以一定要认真的分析需求）；
按照下图的顺序点击，我们就会得到一个需求视图
![在这里插入图片描述](https://img-blog.csdnimg.cn/2021020214154632.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
下一步，点击我们新建的需求视图，从左侧工具栏中将角色和需求的表示形状（火柴人，气泡）拖拽到场景中来
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202142205194.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
## 1.逻辑视图

现在我们再把目光移到右边，给模块新建一个逻辑视图
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202142728197.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
逻辑视图建好后再次点击它，开始编辑（==一定要拖拽到图中==）
工程文件

![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202143028610.png)
UML图
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202143151368.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)文件夹画好后点击，在对应文件夹中新建类（录入方法），右键类下拉菜单找到Operations和Attribute开始录入
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202143831988.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202144601148.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)

代码如下（示例）：



```c
 public List<string> getSlaveIPLst()
        {
            return BeanFactoryBE.buConfigInner.getSlaveIPLst();
        }

        /// <summary>
        /// 获得SlaveVo集合(含IsEnable/IsConCopy)
        /// </summary>
        public List<SlaveVo> getSlaveVoLstWithIsEnableAndIsConCopy()
        {
            return BeanFactoryBE.buConfigInner.getSlaveVoLstWithIsEnableAndIsConCopy();
        }

        /// <summary>
        /// 获得SlaveVo(含IsEnable/IsConCopy)
        /// </summary>
        public SlaveVo getSlaveVoWithIsEnableAndIsConCopy(string strDevType)
        {
            return BeanFactoryBE.buConfigInner.getSlaveVoWithIsEnableAndIsConCopy(strDevType);
        }
```
录好后的UML类图如下
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202144742275.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)

## 3.时序图
在UML中还有一个很重要的图，能清楚的表达模块的逻辑调用关系，那就是时序图
这样在逻辑视图中新建一个逻辑视图，并点击，开始编辑
![在这里插入图片描述](https://img-blog.csdnimg.cn/2021020214511052.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
将右侧，我们已经录入完的类拖拽到图中
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202145425195.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
为展示模块的调用关系我们用左侧Message连接类和被调用类
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202145527492.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
选择调用的具体方法
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202145650988.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
如图，将每个类都画好
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202145823809.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
最后我们要为进程生命线结尾添加返回参，还是用上面的箭头反方向连接两个类的生命线，表示回参，勾选is return（如果这个方法有返回值要添加）
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202150118436.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
最后
![在这里插入图片描述](https://img-blog.csdnimg.cn/20210202150154337.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzc5ODcxNQ==,size_16,color_FFFFFF,t_70)
这样一个简单的UML图就画完了！
==谢谢你一直看到了这里，想必你也是刚参加工作，或刚熟悉编程，那么让我们一起加油吧！==







# 总结
上面内容多图，可能会眼花，最后简单总结一下：
1.先理解工程架构
2.熟悉工程文件的逻辑
3.分析需求
4.绘制需求视图
5.绘制逻辑视图
6.录入类和方法
7.绘制时序图

