# character-gallery



# 小白经历

git push -u origin main 为什么还要通过git和浏览器, 为什么不能想scp一样直接上次呢??

再次添加了语音播放功能, 在chatgpt的协助下, 真的很简单, 这样学习效率也高. 从游戏中提取并找合适的音频反而是最花时间的.

现在搞明白了, 原来git fetch/clone 与 push分成了https与ssh两套东西.
git remote add origin xxxxx 在设置这个xxxxx时分成了https与ssh.
git remote -v可以查看, git remote set-url origin git@github.com:username/repository.git 可以修改https与ssh
没人指导和询问真的要走好多弯路, 我之前一直以为是网络, vpn代理等问题.

又添加背景音乐, 感觉代码逻辑并不难, 前端更像是一种体力活和艺术活, 对数学逻辑要求不高.

功能可以不断更新, 把自己的想法都实现, 但是再搞这个就太花时间了, 主要是提取音频文件, 再通过ffmpeg转化压缩等等花时间. 设计层面我以简洁为中心, 开始还设计一个播放按钮什么的, 但是太难看了.

这会儿好烦, git push  与 git pull, 以及git那个学习, 感觉主要还是要实用为主, 为了学而学很不好.
