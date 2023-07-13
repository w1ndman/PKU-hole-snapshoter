# PKU-hole-snapshoter

保存树洞快照，在被删帖时从快照中获取最新版本并恢复
此插件目前只会在用户刷新时保存数据，并不会主动向服务器发送请求，而且目前没有加入主动发送请求的开发计划
已经实现的功能：
- 缓存树洞内容以及评论回复
- 在刷新时若发现有被删除的帖子，查找本地储存，若发现有备份，则将数据插入至数据包中

效果图：
![16211689227937_ pic](https://github.com/w1ndman/PKU-hole-snapshoter/assets/132929861/a4dd7f9f-f980-456a-a501-162f858649be)



**本脚本只能恢复之前获取过的数据，换句话说，只能恢复之前通过正在使用的这个浏览器窗口看过的树洞**

## TODO:
- [ ] 修复潜在bug（很可能会有）
- [ ] 一些代码整理（尝试美化屎山）
- [ ] 加入恢复单个被删除评论的功能，（目前只有备份功能）
- [ ] 目前储存数据的位置是local storage，上限为10M左右，所以计划未来将储存位置换成indexedDB，
- [ ] 加入用户交互部分，比如一些开关按钮
- [ ] （可能的一个方向）将数据库扩展至服务器上，比如从GitHub上拉取和上传树洞数据备份

油猴脚本：[https://greasyfork.org/zh-CN/scripts/470731-pku-hole-snapshoter](https://greasyfork.org/zh-CN/scripts/470731-pku-hole-snapshoter)
