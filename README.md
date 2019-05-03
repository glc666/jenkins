# Jenkins 入门 
## Jenkins 安装
1、安装JDK
JDK若已经安装者跳过
```
yum install -y java
```
2、下载jenkins
```
wget http://pkg.jenkins-ci.org/redhat-stable/jenkins-2.7.3-1.1.noarch.rpm
rpm -ivh jenkins-2.164.2-1.1.noarch.rpm
```

3、配置jenkis的端口(可选)
找到修改端口号：

JENKINS_PORT="8080"  此端口不冲突可以不修改 

```
 vi /etc/sysconfig/jenkins
```


4、启动jenkins
```
service jenkins start/stop/restart
```
安装成功后Jenkins将作为一个守护进程随系统启动
系统会创建一个“jenkins”用户来允许这个服务，如果改变服务所有者，同时需要修改/var/log/jenkins, /var/lib/jenkins, 和/var/cache/jenkins的所有者
启动的时候将从/etc/sysconfig/jenkins获取配置参数
默认情况下，Jenkins运行在8080端口，在浏览器中直接访问该端进行服务配置
Jenkins的RPM仓库配置被加到/etc/yum.repos.d/jenkins.repo

5、打开jenkins 

在浏览器中访问 
首次进入会要求输入初始密码如下图， 
初始密码在：/var/lib/jenkins/secrets/initialAdminPassword 

![jenkins-1.png](https://github.com/glc666/jenkins/blob/master/jenkins-1.png "jenkins-1.png")
![jenkins-2.png](https://github.com/glc666/jenkins/blob/master/jenkins-2.png "jenkins-2.png")
![jenkins-3.png](https://github.com/glc666/jenkins/blob/master/jenkins-3.png "jenkins-3.png")
![jenkins-4.png](https://github.com/glc666/jenkins/blob/master/jenkins-4.png "jenkins-4.png")
![jenkins-5.png](https://github.com/glc666/jenkins/blob/master/jenkins-5.png "jenkins-5.png")


、、、
