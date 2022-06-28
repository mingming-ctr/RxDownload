安装过程
1. 保证网络正常，能够正常访问github
2. 安装git
3. 通过git从github上获取源码
4. 开发语言是kotlin,下载安装android sudio集成开发环境
5. 准备手机opp,设置成开发者模式
6. 根据提示处理各种bug,处理核心是不要改源码和配置
7. 能够在opp手机里面看到运行的程序，正常运行

bug以及处理

1. 8:30	Error
		Installation did not succeed.
		The application could not be installed: INSTALL_FAILED_TEST_ONLY
    ![image](https://user-images.githubusercontent.com/12455138/176066035-d73edfe8-3252-4ca0-b614-b2963e4b5d21.png)
处理
参考 https://blog.csdn.net/luo4566/article/details/89642540
gradle.properties文件中添加设置
android.injected.testOnly=false
文件不存在可以参考
https://www.cxyzjd.com/article/w2_2015/110166128
我是直接拷贝新项目的gradle.properties,然后设置testOnly

2. 缓存清理

运行中可能存在各种问题，很多是缓存引起的，如下清理
![image](https://user-images.githubusercontent.com/12455138/176067914-e915edd5-d1bd-4b89-8994-6dc225746952.png)



运行效果

![image](https://user-images.githubusercontent.com/12455138/176086970-fbd048b0-4fee-45d4-8f8b-9e3269162543.png)
![image](https://user-images.githubusercontent.com/12455138/176086982-45a54cde-9f24-499b-bd29-f7d68ae8df11.png)
![image](https://user-images.githubusercontent.com/12455138/176086991-9d532c51-6fd5-4f00-8567-97df6f087633.png)
![image](https://user-images.githubusercontent.com/12455138/176087016-75f9427b-4ae7-4168-90fe-2eda88348cb0.png)
![image](https://user-images.githubusercontent.com/12455138/176087035-13bd52ee-ec2c-4a60-b783-9b998ab9a88a.png)
![image](https://user-images.githubusercontent.com/12455138/176087050-6b4d396e-0b9a-43b8-9f07-5e3738d5d3f4.png)

需要的可以在上面加入自己的功能。


