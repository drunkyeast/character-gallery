# character-gallery

git push -u origin main 为什么还要通过git和浏览器, 为什么不能想scp一样直接上次呢??

成功push了.

额外补充了一些图片

再次添加了语音播放功能, 在chatgpt的协助下, 真的很简单, 这样学习效率也高. 从游戏中提取并找合适的音频反而是最花时间的.

这个git push又出问题了, 哎~

本地电脑修改

现在搞明白了, 原来fetch/clone 与 push分成了https与ssh两套东西.
git remote add origin xxxxx 在设置这个xxxxx时分成了https与ssh.
git remote -v可以查看, git remote set-url origin git@github.com:username/repository.git
没人指导和询问真的要走好多弯路, 我之前一直以为是网络, vpn代理等问题.

我现在再本来电脑中先修改README.md再pull, 此时显示both modified, 再push.

我现在再vps中pull了下来, 此时显示modified, 我修改一下README.md在pull.

又添加扩展了语音功能, 可以播放一到两个音频. 我还想进一步添加背景音乐.

又添加背景音乐, 感觉代码逻辑并不难, 前段更像是一种体力活和艺术活, 对数学逻辑要求不高.

功能可以不断更新, 把自己的想法都实现, 但是再搞这个就太花时间了, 主要是提取音频文件, 再通过ffmpeg转化压缩等等花时间. 设计层面我以简洁为中心, 开始还设计一个播放按钮什么的, 但是太难看了.

这会儿好烦, git push  与 git pull 用的还是挺好用的.
