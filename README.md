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

我现在再本来电脑修改并push, 并从vps pull.
