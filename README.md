## character-gallery
这是静态网页. 用json文件写下老婆们的个人信息, 立绘路径, 音频路径. 然后html和css文件加载json的信息, 把老婆们展示在静态页面中. 是我看了谷雨同学的网站后参考着做的.
代码实现不难, 全靠chatgpt, 但代码不太优雅. 我时间主要花在了找立绘和音频, 提取游戏中的立绘和音频. 尤其是加藤惠那张立绘, 全网唯一, 我自己做的, 把腿拼接上去的.

部署的话, 就是把整个目录放到/var/www/下面, nginx默认是那里的. 然后配置nginx.conf等相关信息, ssl证书等.


## 更新记录
### 23年8月, 在chatgpt的帮助下实现了第一个版本, 代码不太好看, 都是chatgpt写的. 其实也是第一次自己做的小项目, git都不太会用. 下面是当时的一些吐槽: 
小白记录

git push -u origin main 为什么还要通过git和浏览器, 为什么不能想scp一样直接上次呢??

再次添加了语音播放功能, 在chatgpt的协助下, 真的很简单, 这样学习效率也高. 从游戏中提取并找合适的音频反而是最花时间的.

现在搞明白了, 原来git fetch/clone 与 push分成了https与ssh两套东西.
git remote add origin xxxxx 在设置这个xxxxx时分成了https与ssh.
git remote -v可以查看, git remote set-url origin git@github.com:username/repository.git 可以修改https与ssh
没人指导和询问真的要走好多弯路, 我之前一直以为是网络, vpn代理等问题.

又添加背景音乐, 感觉代码逻辑并不难, 前端更像是一种体力活和艺术活, 对数学逻辑要求不高.

功能可以不断更新, 把自己的想法都实现, 但是再搞这个就太花时间了, 主要是提取音频文件, 再通过ffmpeg转化压缩等等花时间. 设计层面我以简洁为中心, 开始还设计一个播放按钮什么的, 但是太难看了.^S

这会儿好烦, git push  与 git pull, 以及git那个学习, 感觉主要还是要实用为主, 为了学而学很不好.

### 23年12月
修改了背景图片的透明度, 添加了新老婆加藤惠, 修改了json. 备份了原来的json文件.

我用https下载的这个项目, 所以我在git push时用的https认证, 要用账户密码验证, 另外就算输了也显示fatal:...失败. 
`git remote -v`查看用的https还是SSH.
`git remote set-url origin git@github.com:username/repository.git` 将https认证改成SSH, 然后把公钥添加到github.

### 24年7月
添加阿良良木月火, 现在逐渐感觉文件变大了, 后续考虑如何压缩等优化. 以及对json添加一个属性, 可以调节音频大小, 不然手动ffmpeg再scp好麻烦, 真是让人白金火大!.
现在对各种音视频文件格式有一个简单的了解了, 后续优化可以考虑同一格式.
