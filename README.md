#社团网改版需求

2016-5-17

##目前社团网架构
1. 首页
    - 轮播图（静态展示，需要手动添加图片，没有链接和文字）
    - 新闻（四个色块展示前四个最新新闻，无图片）
    - 五个快捷链接
        - 资料下载（无链接，理论上对应后台资料下载栏目）
        - 设计委任(Design/Index/index)，目前尚在改版
        - 资源申请(Material/Index/index)
        - 评分系统(Grade/Index/index)
        - 社团卡(AssociationCard/Index/index)纯静态页面展示
2. 新闻
  1. 最新动态(也即新闻版块)
    - 文章分类
    - 文章属性
    - 文字标题
    - 文章正文(html富文本)
  2. 活动预告
    - 预告内容(目前为纯文本，可扩展为html富文本)
    - username发布者用户名
    - 地点(纯文本)
    - 时间(int10，时间戳格式)
  3. 通知公告
    - 通知内容(目前为纯文本，可扩展为html富文本)
    - 发布者账户id(uid)
    - 时间(int10，时间戳格式)

3. 社团
    - 目录页+一堆静态社团介绍页面

##总体策划要求
1. 确定总基调，配色、页面元素等偏向活泼风格，不要太过xing冷淡
2. 在现有架构的基础上，尽量减少对架构的大型修改，用脑图等形式建立社团网的总体架构
3. logo使用**新**社联标志+社团网类似字样
4. 考虑与当前网站的兼容
5. 给出首页、新闻展示页面的示意图或产品原型
6. PC端+手机端

##具体页面及元素要求
主题色：绿色

**貌似并没有限定过具体RGB颜色，因此按照Google Material Design给出的Green，Light green调色板**

**默认主色调为Green 500:#4caf50**

![请走传送门查看](http://o79pnjsg2.bkt.clouddn.com/sicun/201605/aunet/redesign/intro/materialdesign-color.png)

    * Green 500 
    * 50#E8F5E9
    * 100#C8E6C9
    * 200#A5D6A7
    * 300#81C784
    * 400#66BB6A
    * 500#4CAF50
    * 600#43A047
    * 700#388E3C
    * 800#2E7D32
    * 900#1B5E20
    * A100#B9F6CA
    * A200#69F0AE
    * A400#00E676
    * A700#00C853

    * Light Green500#8BC34A
    * 50#F1F8E9
    * 100#DCEDC8
    * 200#C5E1A5
    * 300#AED581
    * 400#9CCC65
    * 500#8BC34A
    * 600#7CB342
    * 700#689F38
    * 800#558B2F
    * 900#33691E
    * A100#CCFF90
    * A200#B2FF59
    * A400#76FF03
    * A700#64DD17

传送门：
Google Official 
[https://www.google.com/design/spec/material-design/introduction.html](https://www.google.com/design/spec/material-design/introduction.html)
Color [https://www.google.com/design/spec/style/color.html](https://www.google.com/design/spec/style/color.html)

###统一设计

**以下所有栏目都是建议栏目，请根据设计自行调整**

1. 导航栏
    - logo（社团网）
    - 链接
    - 登录按钮
2. 页脚
    - 友情链接
    - 联系方式
    - 微信公众号二维码
    - Copyright行
    
3. 统一登录模块
    - 用户名
    - 密码
    - 验证码
    - 登录按钮
    - 最底部copyright
    - **后台注意** 所有需登录模块（后台、物资系统、传媒委任等）的登录页面转至此统一登录模块，可通过URL传参或设定session等方式确定登录后跳转页面

###分页面

1. 首页
    - 导航栏
    - 轮播图
        - 图片+文字+链接（可选）
        - 图片确定比例（如16:9），最小可接受分辨率，可加入后台管理
    - 新闻（链接到文章）
        - 图片+标题+缩略文字（图片选用文章第一张图片，无则用默认图片替代）
        - 时间（可选）
    - 活动预告（链接到文章）
        - 名称
        - 时间
        - 地点
        - 简介
        - 举办方
    - 通知（链接到文章）
        - 标题
    - 快速链接
        - 物资申请
        - 传媒委任
        - 评分系统
        - 人资管理
        - 社团卡
        - 资料下载
        - ...
    - 文件下载（快捷链接区域）（可公开的文件）
    - 其他小栏目（可选，仅供参考）
        - 社团风采
        - 会员、会长风采
        - 简略FAQ

2. 新闻、预告、通知页面
    - 正文区域
        - 标题
        - 时间
        - 文章分类（新闻 预告 通知）
        - 文章属性
        - 文章正文
    - 侧边栏
        - 分类（新闻 预告 通知）
        - 属性（以tag的形式）
            

##参考材料
###同类网站
1. 清华大学 [http://shetuan.student.tsinghua.edu.cn/](http://shetuan.student.tsinghua.edu.cn/)
2. 浙江大学 [http://www.cde.zju.edu.cn/](http://www.cde.zju.edu.cn/)

###模板网站
1. jekyll theme [http://jekyllthemes.org/](http://jekyllthemes.org/)
2. Hexo theme [https://hexo.io/themes/](https://hexo.io/themes/)
3. Bootstrap themes [http://themes.getbootstrap.com/](http://themes.getbootstrap.com/)
4. Material Design [https://getmdl.io/templates/index.html](https://getmdl.io/templates/index.html)
5. Bootstrap优站精选 [http://expo.bootcss.com/](http://expo.bootcss.com/)


