> dede_addonarticle：附加文章表 
```
aid int(11) 文章编号 
typeid int(11) 分类栏目编号 
body mediumtext 文章内容 
dede_addonflash 附加Flash表 
aid int(11) FLASH编号 
typeid int(11) 分类栏目编号 
filesize varchar(10) 文件大小 
playtime varchar(10) 播放时长 
flashtype varchar(10) 作品类型 
flashrank smallint(6) 作品等级 
width smallint(6) 影片宽度 
height smallint(6) 影片高度 
flashurl varchar(80) FLASH地址 
```


> dede_addonimages： 附加图集表 
```
aid int(11) 图集编号 
typeid int(11) 分类栏目编号 
pagestyle smallint(6) 表现方式（1单页显示 2分多页显示 3多行多列展示） 
maxwidth smallint(6) 大图限制宽度 
imgurls text 图片集内容（标签存放） 
row smallint(6) 多列式参数（行） 
col smallint(6) 多列式参数（列） 
isrm smallint(6) 是否下载远程图片 
ddmaxwidth smallint(6) 小图片宽度限制
``` 


> dede_addonsoft 附加软件表 
```
aid int(11) 软件编号 
typeid int(11) 分类栏目编号 
filetype varchar(10) 文件类型 
language varchar(10) 界面语言 
softtype varchar(10) 软件类型 
accredit varchar(10) 授权方式 
os varchar(30) 运行环境 
softrank int(11) 软件等级 
officialUrl varchar(30) 官方网址 
officialDemo varchar(50) 程序演示地址 
softsize varchar(10) 软件大小 
softlinks text 软件下载链接列表 
introduce text 软件介绍
```
 
> dede_addonspec： 附加专题表 
```
aid int(11) 专题编号 
typeid int(11) 分类栏目编号 
note text 专题内容（仅存放标签代码） 
```

> dede_admin： 管理员信息表 
```
ID int(10) 自动编号 
usertype int(10) 用户类型 
userid varchar(30) 用户登录ID 
pwd varchar(50) 用户密码 
uname varchar(20) 用户笔名 
tname varchar(30) 真实姓名 
email varchar(30) 电子邮箱 
typeid int(11) 负责频道（0表示全部） 
logintime datetime 登录时间 
loginip varchar(20) 登录IP
```
 
> dede_admintype ：系统用户组管理表 
```
rank smallint(6) 组级别编号 
typename varchar(30) 组名称 
system smallint(6) 是否为系统默认组 
purviews text 权限列表 
```

> dede_arcatt ：文档自定义属性表 
```
att smallint(6) 编号 
attname varchar(30) 属性名称 
dede_archives 文章表 
ID int(11) 自动编号 
typeid int(11) 所属主栏目编号 
typeid2 int(11) 所属副栏目编号 
sortrank int(11) 文章排序（置顶方法） 
iscommend smallint(6) 是否推荐 
ismake smallint(6) 是否生成静态 
channel int(11) 文章所属模型 
arcrank smallint(6) 阅读权限 
click int(11) 点击次数 
money smallint(6) 消费点数 
title varchar(80) 标题 
shorttitle varchar(36) 简略标题 
color varchar(10) 标题颜色 
writer varchar(30) 作者 
source varchar(50) 来源 
litpic varchar(100) 缩略图 
pubdate int(11) 录入时间 
senddate int(11) 发布时间 
arcatt smallint(6) 自定属性（att） 
adminID int(11) 发布管理员ID 
memberID int(11) 发布会员ID 
deｓｃｒｉｐｔion varchar(250) 摘要 
keywords varchar(60) 关键词 
templet varchar(60) 文档模板 
lastpost int(11) 最近评论时间 
postnum int(11) 评论数目 
redirecturl varchar(150) 跳转网址 
mtype int(11) 用户自定义分类 
userip varchar(20) 用户IP 
locklikeid smallint(6) 是否锁定相关文章 
likeid varchar(240) 相关文章ID 
```

> dede_arcrank： 阅读权限表 
```
ID int(10) 自动编号 
rank smallint(10) 权限等级 
membername varchar(20) 等级名称 
adminrank smallint(10) 管理等级 
money int(11) 消费点数
```
 
> dede_arctype ：栏目管理表 
```
ID int(10) 栏目编号（自动编号） 
reID int(10) 父栏目编号 
topID int(10) 　 
sortrank smallint(6) 排序编号 
typename varchar(30) 栏目名称 
typedir varchar(100) 栏目目录 
isdefault smallint(6) 栏目列表选项（1链接到默认页 0链接到列表第一页 -1使用动态页） 
defaultname varchar(20) 默认页的名称 
issend smallint(6) 是否支持投稿 
channeltype smallint(6) 频道类型 
maxpage int(11) 保留 
ispart smallint(6) 栏目属性 
corank smallint(6) 浏览权限 
tempindex varchar(60) 封面模板 
templist varchar(60) 列表模板 
temparticle varchar(60) 文章模板 
tempone varchar(60) 单独页面模板 
namerule varchar(50) 文章命名规则 
namerule2 varchar(50) 列表命名规则 
modname varchar(30) 模板名称 
deｓｃｒｉｐｔion varchar(200) 栏目介绍 
keywords varchar(100) 关键词 
moresite smallint(6) 多站点支持 
siterefer smallint(6) 多站点站点根目录属性 
sitepath varchar(60) 多站点站点根目录 
siteurl varchar(60) 多站点绑定域名 
ishidden smallint(6) 是否隐藏栏目 
```

> dede_area： 地区表 
```
eid int(11) 地区编号 
name varchar(20) 地区名称 
rid int(11) 编号属性
```