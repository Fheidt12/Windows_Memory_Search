# 工具运行界面
![image](https://github.com/user-attachments/assets/c7be3697-ec75-4b95-a310-f4be2fed960a)
免责声明：此工具仅限于安全研究，用户承担因使用此工具而导致的所有法律和相关责任！作者不承担任何法律责任

## 检索指定字符串
例如：123456.dnslog.cn.com（微信中发送这个域名信息）
pid不填写时，会遍历全部进程,将结果pid，进程名，进程路径表格形式输出

![image](https://github.com/user-attachments/assets/a335869d-306a-4fc1-97aa-e514a0c157b1)


将结果保存至Memory_search_result文件中

![image](https://github.com/user-attachments/assets/a860dd13-5725-4bc5-8378-30d3dc7fce79)



## 指定进程PID进行检索
指定进程检索，会将对应地址对应内存字符部分打印出来，默认长度为50，即可确认，相关字符串的前后的具体操作
![image](https://github.com/user-attachments/assets/0f043fe3-0f47-42db-91e9-302e3efe6384)

## 使用场景  

1、webshell中攻击者执行了哪些命令
![image](https://github.com/user-attachments/assets/b533022f-c67d-41df-b018-057f29cf1f79)

2、攻击者是否执行了mimikat抓取密码
![image](https://github.com/user-attachments/assets/6854d940-a05b-46ca-b660-ec944ed7d7f5)

3、按照该上面测试，只要知道了攻击者恶意进程（通过外联啊 特征字符串定位），就可以看攻击者的历史操作记录，前提是服务器没有重启过  

4、内存马应该也可以定位，目前没有测试，感兴趣的同学可以自己测试下

## 说明
1、有同学反馈工具下载360会报毒，报毒原因为360qvm引擎检测到程序没有签名，因此产生报毒；下载后的文件，对比md5相同即可使用

2、工具开发思路：https://www.freebuf.com/sectool/408673.html 里面有具体的api使用说明，由于工具暂时处于测试阶段，暂不开发源码
