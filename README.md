[![clean version](https://img.shields.io/badge/release-v1.1-blue.svg)](https://github.com/caviare/clean/releases)
[![ghost version](https://img.shields.io/badge/ghost-v3.12.1-brightgreen.svg)](https://github.com/TryGhost/Ghost/releases)

## clean

clean 是一个简洁清新的 ghost 博客现代主题，你可以在我的[博客](https://www.imcaviare.com)看到它。

![](https://ww1.sinaimg.cn/large/005M2kKhly1fy4v6idun0j318g0tjdst.jpg)

![](https://ww1.sinaimg.cn/large/005M2kKhly1fy4v7agyghj318g0tn79h.jpg)

### 功能简介

---

- gitalk 评论
- 增加归档页面
- 标签筛选文章
- 兼容 ghosV3 版本
- 兼容移动端

### gitalk 评论正确食用方法

---

在后台中博客页面顶部声明[gitalk](https://github.com/gitalk/gitalk)配置，以下是我的[gitalk](https://github.com/gitalk/gitalk)配置示例：

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdkyyz2uxhj33n01la4e3.jpg)

### 增加归档页

1. 下载路由
2. 修改路由
   - 在 routes 下增加归档页面**tag**
   ```yaml
   routes:
     /tag/: tag
   ```
3. 将修改好的路由文件上传

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdl2im6faoj33h61m2dsa.jpg)

4. 显示归档也到导航栏

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdkze8e18wj33xg1nc4qq.jpg)

### 增加留言页面与关于我的页面

---

- 在 ghost 后台增加页面

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdl5s093nbj33rs1oik0h.jpg)

- 如果要使用 gitalk，在页面底部加入以下代码

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

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdl5s0hilsj33wo1scwy1.jpg)

- 在 page 设置中设置页面路由

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdl5s0twahj33vi1naax9.jpg)

- 在 ghost 导航设置中加上我们增加的页面

![](https://ww1.sinaimg.cn/large/005M2kKhly1gdkze8e18wj33xg1nc4qq.jpg)
