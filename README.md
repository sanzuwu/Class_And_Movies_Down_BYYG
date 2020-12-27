# 软件介绍
  * 1、如果需要下载付费的视频，需要先购买后在cookie.json中填写好cookie读取的路径，并新建对应文件名的txt粘贴cookie
  * 2、软件按照课程大纲下载，按顺序下载课程大纲下所有视频，无cookie时收费视频将会被跳过
  * 3、部分网校需要填写token才能下载，如需要的会额外提示
  * 4、在任意的等待输入状态下，输入@后回车可以强制返回上一级
  * 5、现在可以下载单个视频，获取完课程列表后，输入序号后回车会下载对应序号的视频，不输入直接回车下载全部视频
  * 序号可以使用英文逗号分开多段，可以使用减号设置区间，例如输入 0-3，5，9，47-59
  * 则表示下载第0到第3，第5，第9，第47到第59的视频
  * 6、软件支持断点续传，已下载的视频不会重复下载
  * 7、使用方法在软件内会有提示


# 软件下载地址
软件地址：https://www.lanzoux.com/b00z8zafe

# 抓取已购买课程的cookie
购买课程后，在浏览器中按F12，在Network标签下F5刷新，然后点击第一个，找到headers标签下的cookie，全部复制粘贴到cookie.txt下，就可以下载付费的课程

![抓取截图](https://attach.52pojie.cn/forum/202009/19/211335u7f6s7qy1fhuurr4.jpg)  

# cookie编辑
```
{
    "1":{
        "cookie":"51cto"
    },
    "2":{
        "cookie":"muke"
    },
    "12":{
        "cookie":"wanmen",
        "token":"wanmentk"
    }
}
```
前面的键代表软件内的序号，例如1代表序号1功能读取这部分内容，【"cookie":"51cto"】代表当序号1功能需要读取cookie时，将会读取同目录下的51cto.txt的内容作为这个序号功能的cookie。
例如最后的12，【"cookie":"wanmen"】代表当序号12功能需要读取cookie时，将会读取同目录下的wanmen.txt的内容作为这个序号功能的cookie；【"token":"wanmentk"】代表当序号12功能需要读取token时，将会读取同目录下的wanmentk.txt的内容作为这个序号功能的token
默认所有键名都为cookie，如需要token时会额外进行提示
备注：在进行cookie配置文件编辑时，建议使用https://www.json.cn进行编辑，编辑完成后再复制到【cookie.json】内保存

![抓取截图](https://attach.52pojie.cn/forum/202011/11/200938c6053573mmm3m5yw.jpg)  
