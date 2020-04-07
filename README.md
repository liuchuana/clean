
[![clean version](https://img.shields.io/badge/release-v1.1-blue.svg)](https://github.com/caviare/clean/releases)
[![ghost version](https://img.shields.io/badge/ghost-v3.12.1-brightgreen.svg)](https://github.com/TryGhost/Ghost/releases)

## clean
---
clean是一个简洁清新的ghost博客现代主题，你可以在我的[博客](https://www.imcaviare.com)看到它。


### 功能简介
---
- gitalk评论
- 增加归档页面
- 标签筛选文章
- 兼容ghosV3版本
- 兼容移动端

### gitalk评论正确食用方法
---

在后台中博客页面顶部声明[gitalk](https://github.com/gitalk/gitalk)配置，以下是我的[gitalk](https://github.com/gitalk/gitalk)配置示例：

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdkyyz2uxhj33n01la4e3.jpg)

### 关于增加留言页面与关于我的页面
---
在ghost后台增加页面

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdkz58j4qfj33rs1oik0h.jpg)

如果要使用gitalk，在页面底部加入以下代码
```javascript
    <script type="text/javascript">
        window.onload=function(){
            if (gitalkConfig) {
                var gitalk = new Gitalk(gitalkConfig)
                gitalk.render('gitalk-container')
            }  
        }
    </script>
```

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdkzbamhkgj33wo1scwy1.jpg)

在page设置中设置页面路由

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdkz1z6bw9j33vi1naax9.jpg)

在ghost导航设置中加上我们增加的页面
![](http://ww1.sinaimg.cn/large/005M2kKhly1gdkze8e18wj33xg1nc4qq.jpg)