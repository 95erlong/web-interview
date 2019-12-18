### SEO
  什么是 SEO
  百度百科：
    SEO (Search Engine Optimization): 搜索引擎优化。搜索引擎优化是一种利用搜索引擎的搜索规则来提高目前网站有关搜索引擎内的自然排名的方式。SEO 是为了从搜索引擎中获得更多的免费流量，从网站结构、内容创建方案、用户互动传播、页面等角度进行合理规划，使网站更合适搜索引擎的索引原则的行为
  
  SEO 原理
    页面抓取：蜘蛛向服务器请求页面，获取页面内容
    分析入库：对获取到的内容进行分析，对优质页面进行收录
    检索排序：当用户检索关键词时，从收录的页面中按照一定的规则进行排序，并返回给用户结果
  
  SEO 优化
    页面抓取：
      如何才能吸引蜘蛛光顾我们的网站，如何才能让蜘蛛经常光顾我们的网站。这里提出一下几个优化点：
      
      1.提交页面。提交页面又分为几种不同的方式
        1.sitemap 提交。sitemap，顾名思义，就是网站地图，当蜘蛛来到我们的网站时，告诉它我们有多少页面，不同页面是按什么分类的，每个页面的地址是什么。顺着我们的指引，蜘蛛会很轻松的爬遍所有内容。另外如果你的页面分类比较多，而且数量大，建议添加 sitemap 索引文件。如果站点经常更新添加新页面，建议及时更新 sitemap 文件；
        2.主动提交。就是把你的页面直接丢给百度的接口，亲口告诉百度你有哪些页面，这是效率最高也是收录最快的方式。但是需要注意，百度对每天提交的数量是有限制的，而且反复提交重复的页面，会被降低每日限额，所以已被收录的页面不建议反复提交。收录有个时间过程，请先耐心等待；
        3.实时提交。在页面中安装百度给的提交代码，当这个页面被用户打开，便自动把这个页面提交给百度。
     
    前端需要注意哪些 SEO
      1.合理的 title、description、keywords；搜索对这三项的权重逐个减小，title 值强调重点即可，重要关键词出现不要超过 2 次，而且要靠前，不同页面 title 要有所不同；description 把页面内容高度概括，长度合适，不可过分堆砌关键词，不同页面 description 有所不同；keywords 列举出重要关键词即可。
      2.语义化的 HTML 代码，符合 W3C 规范：语义化代码让搜索引擎容易理解网页
      3.重要内容 HTML 代码放在最前面：搜索引擎抓取 HTML 顺序是从上到下，有的搜索引擎对抓取长度有限制，保证重要内容一定会被抓取
      4.重要内容不要用 js 输出：爬虫不会执行 js 获取内容
      5.少用 iframe：搜索引擎不会抓取iframe中的内容
      6.非装饰性图片必须加 alt
      7.提高网站速度：网站速度是搜索引擎排序的一个重要指标
      
### web 开发中会话跟踪的方法有哪些
  1.cookie
  2.session
  3.URL 重写
  4.隐藏 input
  5.IP 地址

### img 的 title 和 alt 有什么区别
  1.title 是 global attributes 之一，用于为元素提供附加的 advisory information。通常当鼠标滑动到元素上的时候显示。
  2.alt 是 img 的特有属性，是图片内容的等价描述，用于图片无法加载时显示、读屏器阅读图片。可提高图片可访问性，除了纯装饰图片外都必须设置有意义的值，搜索引擎会重点分析。
  
### doctype 是什么，举例常见 doctype 及特点
  1.<!doctype> 声明必须处于 HTML 文档的头部，在 html 标签之前， HTML 5 中不区分大小写
  2.<!doctype> 声明不是一个 HTML 标签，是一个用于告诉浏览器当前 HTML 版本的指令
  3.现代浏览器的 html 布局引擎通过检查 doctype 决定使用兼容模式还是标准模式对文档进行渲染，一些浏览器有一个接近标准模型
  4.在 HTML 4.01 中 <!doctype> 声明指向一个 DTD，由于 HTML 4.01 基于 SGML，所以 DTD 指定了标记规则以保证浏览器正确渲染内容
  5.HTML5 不基于 SGML，所以不用指定 DITD
  
  常见 doctype
    1. HTML4.01 strict：不允许使用表现性、废弃元素（如 font）以及 frameset。声明：<!DOCTPYE HTML PUBLIC"-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    2.HTML4.01 Transitional：允许使用表现性、废弃元素（如 font），不允许使用 frameset。声明：<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd" >
    3.HTML4.01 Frameset：允许表现性元素，废弃元素以及 frameset。声明：<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd" >
    4.XHTML1.0 Strict：不允许使用表现性、废弃元素以及 frameset。文档必须是结构良好的 XML 文档。声明 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd" >
    5.XHTML1.0 Transitional：允许使用表现性、废弃元素，不允许 frameset，文档必须是结构良好的 XML 文档。声明：<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd" >
    6.XHTML1.0 Frameset：允许使用表现性、废弃元素以及 frameset，文档必须是结构良好的 XML 文档。声明：<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd" >
    7.HTML5: <!doctype html >
    

### HTML 全局属性有哪些
  1.accesskey：设置快捷键，提供快速访问元素如 aaa 在 windows 下的 firefox 中按 alt + shift + a 可激活元素
  2.class：为元素设置类标识，多个类名用空格分开，CSS 和 Javascript 可通过 class 属性获取元素
  3.contenteditable：指定元素内容是否可编辑
  4.contextmenu：自定义鼠标右键弹出菜单内容
  5.data-*：为元素增加自定义属性
  6.dir：设置元素文本方向
  7.draggable：设置元素是否可拖拽
  8.dropzone：设置元素拖放类型：copy、move、link
  9.hidden：表示一个元素是否与文档。样式上会导致元素不显示，但是不能用这个属性实现样式效果
  10.id：元素 ID，文档内唯一
  11.lang：元素内容的语言
  12:spellcheck：是否启动拼写和语法检查
  13.style：行内 css 样式
  14.tabindex：设置元素可以获得焦点，通过 tab 可以导航
  15:title：元素相关的建议信息
  16:translate：元素和子孙节点内容是否需要本地化


### 什么是 web 语义化，有什么好处
  web 语义化是指通过 HTML 标记表示页面包含的信息，包含了 HTML 标签的语义化和 css 命名的语义化。HTML 标签的语义化是指：通过使用包含语义的标签（如 h1-h6），恰当地表示文档结构 css 命名的语义化是指：为 html 标签添加有意义的 class，id 补充未表达的语义，
  为什么需要语义化：
  1.去掉样式后页面呈现清晰的结构
  2.盲人使用读屏器更好地阅读
  3.搜素引擎更好的理解页面，有利于收录
  4.方便团队项目的可持续运作及维护
  
### HTTP method
  1.一台服务器要与 HTTP1.1 兼容，只要为资源实现 GET 和 HEAD 方法即可
  2.GET 是最常用的方法，通常用于请求服务器发送某个资源
  3.HEAD 与 GET 类似，但服务器在相应中只返回首部，不返回实体的主体部分
  4.PUT 让服务器用请求的主体部分来创建一个由所请求的 URL 命名的新文档，或者，如果那个 URL 已经存在的话，就用这个主体替代它
  5.POST 起初是用来向服务器输入数据的。实际上，通常会用它来支持 HTML 的表单。表单中填好的数据通常会被送给服务器，然后由服务器将其发送到要去的地方
  6.TRACE 会在目的服务器端发起一个环回诊断，最后一站的服务器会弹回一个 TRACE 响应并在响应主体中携带它收到的原始请求报文。TRACE 方法主要用于诊断，用于验证请求是否如愿穿过了请求/响应链
  7.OPTIONS 方法请求 web 服务器告知其支持的各种功能。可以查询服务器支持哪些方法或者对某些特殊资源支持哪些方法。
  8.DELETE 请求服务器删除请求 UTL 指定的资源

### 从浏览器地址栏输入 URL 到显示页面的步骤（以 HTTP 为例）
  1.在浏览器地址栏输入 URL 
  2.浏览器查看缓存，如果请求资源在缓存中并且新鲜，跳转到转码步骤
    a.如果资源未缓存，发起新请求
    b.如果已缓存，检验是否足够新鲜，足够新鲜直接提供给客户端，否则与服务器进行验证。
    c.检验新鲜通常有两个 HTTP 头进行控制 Expires 和 Cache-Control：
      ·HTTP1.0 提供 Expires，值为一个绝对时间表示缓存新鲜日期
      ·HTTP1.1 增加了 Cache-Control:max-age=,值为以秒为单位的最大新鲜时间
  3.浏览器解析 URL 获取协议，主机，端口，path
  4.浏览器组装一个 HTTP（GET）请求报文
  5.浏览器获取主机 ip 地址，过程如下：
    a.浏览器缓存
    b.本机缓存
    c.hosts 文件
    d.路由器缓存
    e.ISP DNS 缓存
    f.DNS 递归查询（可能存在负载均衡导致每次 IP 不一样）
  6.打开一个 socket 与目标 IP 地址，端口建立 TCP 链接，三次握手如下：
    a.客户端发送一个 TCP 的 SYN=1，Seq=X 的包到服务器端口
    b.服务器发回 SYN=1，ACK=X+1，Seq=Y 的响应包
    c.客户端发送 ACK=Y+1，Seq=Z
  7.TCP链接建立后发送 HTTP 请求
  8.服务器接受请求并解析，将请求转发到服务程序，如虚拟主机使用 HTTP Host 头部判断请求的服务程序
  9.服务器检查 HTTP 请求头是否包含缓存验证信息，如果验证缓存新鲜，返回 304 等对应状态码
  10.处理程序读取完整请求并准备 HTTP 响应，可能需要查询数据库等操作
  11.服务器将响应报文通过 TCP 连接发送回浏览器
  12.浏览器接受 HTTP 响应，然后根据情况选择关闭 TCP 连接或者保留重用，关闭 TCP 连接的 四次握手如下：
    a.主动方发送 Fin=1，Ack=Z，Seq=X 报文
    b.被动方发送 ACK=X+1，Seq=Z 报文
    c.被动方发送 Fin=1，ACK=X，Seq=Y 报文
    d.主动方发送 ACK=Y，Seq=X 报文
  13.浏览器检查响应状态码：是否为 1XX，3XX，4XX，5XX，这些情况处理与 2XX 不同
  14.如果资源可缓存，进行缓存
  15.对响应进行解码（例如 gzip 压缩）
  16.根据资源类型决定如何处理（假设资源为 HTML 文档）
  17.解析 HTML 文档，构建 DOM 树，下载资源，构造 CSSOM 树，执行 js 脚本，这些操作没有严格的先后顺序，以下分别解释
  

