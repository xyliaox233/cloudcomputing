## 数据获取

1. 注册一个晋江账号，登录晋江文学城并选择保持登陆一个月。
2. 前往http://chromedriver.storage.googleapis.com/index.html去下载和你的chrome版本最接近的一个chrome driver。（查看版本方法：地址栏输入chrome://version/）
3. 将下载后的文件解压后得到的文件放到chrome的执行文件所在的目录下和python的安装目录下。
4. 复制chrome的用户设置到新的一个文件夹。
5. 打开driver.py，设置参数
   - target_dir 爬取文件输出的目标路径。
   - Driver()的第一个参数：晋江文学城的官网；第二个参数：4.中复制得到的用户设置拷贝的路径。
   - range(x, y, 10) 爬取从x到y页。
   - year=xx 爬取20xx年的内容。其中19是指2019至2020年。
6. 运行main

注：data里是爬取到的数据的示例。

## Spark Streaming

注：本代码为windows环境下spark运行的测试代码，方便使用，集群环境下的代码结构进行过调整，将按照层次划分的代码结构修改为按照命题划分。

1. 在windows环境下完成spark基本配置

2. 命令行spark-shell
3. 进入win_test文件夹，选择streamingDriver文件，直接运行
4. 可以在streamingDriver中更换运行的进程

## 前端展示

### 性向统计展示

EchartsPre/pre.html 2010-2020性向占比饼图展示

EchartsPre/prePlus.html 2010-2019性向数量变化折线图展示

直接使用浏览器打开即可

## 词云图展示

修改presentation.py中的path_to、path_from，然后运行该文件。

运行结果存储在path_to指向的目录下