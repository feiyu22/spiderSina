# spiderSina
## selenium 是一个浏览器自动化测试框架.可以模拟用户的所有操作. ##

#### 由于浏览器的适配性 我使用的是chrome进行测试.其他浏览器可能因为<br>
#### 版本的原因会有一点漏洞 请尽量使用chrome开发

config.json 是配置文件 必须要先配置好才能运行

> 学习地址: [慕课网 selenium 教程][1]
> 开发环境:
> ide:Netbeans
> java包:selenium全家桶,json和jbdc.mysql
> 浏览器驱动:ie,火狐,谷歌,phantomjs(在res文件夹内)

## 爬虫思路: ##
    
>  1. 打开新浪微博首页并登录
>  2. 跳转到你要爬取数据的人的主页
>  3. 触发ajax将一个页面全部显示出来
>  4. 对每一个微博进行判断解析 只获取他本人的微博  
>  5.如果有展开全文就点击点击一下.然后将微博内容插入数据库
>  6. 判断是否有下一页,如果有就到下一页然后进入第四步

### 目前 我测试了3个用户,一个41页1751条的李敖大师,  
### 一个矮大紧6k多条 鸟哥15k都是没有问题的

## 尚未改进 ##
    1.优化速度
    2.phantomjs 有执行bug 其中一个查找元素会有bug会导致延时1.5s.下载还是没问题的.
    3.浏览器适配
    4.错误处理
    5.代码冗余(不会java语言 我要摸索一下)


  [1]: http://www.imooc.com/video/13952
  [2]: https://github.com/buffge/spiderSina
