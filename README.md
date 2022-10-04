# nonebot_plugin_cave

适用于 [Nonebot2](https://nb2.baka.icu/) 的 cave（回声洞）插件  

## 使用方法:  
群回声洞插件，各群友投稿加入回声洞库，可以随机抽取其中内容。
用户投稿回声洞后，会自动推送给审核人（白名单B成员）进行审核，通过审核后，才能加入库中。  
## env配置:  
`WHITE_B_OWNER=["qq号","qq号"] #可更改白名单B的人员，个数不限`   
## 注意:  
- 1.白名单B中的成员必须为bot好友，否则无法推送审核消息！  
- 2.（待补充）
## 命令:    
以下命令需要加 __命令前缀__（默认为/），可自行设置为空  
### 群聊中命令: `/cave`  
- 不含参数，正常获取cave  
- `-g+id` :查看当前id的回声洞内容  
- `-r+id` :移除该id的回声洞  
- `-a+内容（支持图片，文字）` :添加回声洞（需审核） 
- `-c+cd+unit` :更改当前群的冷却时间,cd:数字,unit:`hour`, `min`, `sec` **____中间以空格分隔____**   
- `-h` :获取cave参数帮助菜单和各项的用法（暂不支持）  
- `-m` :获取新增的投稿的审核情况,时间截至到上次获取  
 
### 私聊审核命令: `/setcave`  
- `-t+id` :通过审核    
- `-f+id` :不通过审核    
- `-l` :查看当前未处理的审核序号列表    
- `-e+id` :查看该id审核情况  

## 冷却：
**__冷却时间长短、上次获取cave的时间,均为分群的存储,各群冷却互不影响__**

