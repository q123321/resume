
## 教育经历  
2012/9-2016/6 就读于湖南大学(985)软件院的数字媒体技术专业  
## 学历  
全日制本科 学士学位  英语四级  
## 联系方式
- 联系电话：15575918345
- Email：634098330@qq.com
- 微信：llj8714300
## 个人信息  
- 刘吕健 男 23岁

- 工作经验：一年

- 目前状态： 离职，正在找工作

- 居住地点： 深圳市龙岗区坂田街道

- 应聘职位：前端开发工程师

- 期望薪资：月薪8k~10k

- 期望工作地点：深圳

- Github：https://github.com/q123321

## 工作经历
#### 中软国际科技服务有限公司（2016年6月到2017年3月）
- 工作描述： 
- 利用html+css快速还原设计稿，利用js、jquery、dom实现各种网页特效与交互。
- 利用ajax和jsonp请求数据，当请求数据出现错误时，利用chrome开发工具来查看http报文从而快速定位错误，若错误是后端的问题，及时地与后端沟通。
- 利用webpack、requirejs等工具打包、合并、压缩代码与各种静态资源。
- 当发现页面加载速度过慢时快速定位问题，并对对影响页面性能的地方进行优化以提高页面的加载速度。
## 项目作品
#### 京东云首页
- 对京东云首页进行了还原，基于 react 和 redux 构建 ，采用 es6 语法，用了 class 类、解构赋值、箭头函数、函数默认值、块级作用域等知识。使用 npm、webpack 作为自动化构建工具 es6 转 es5、打包合并代码。
- 在动手开发之前发现京东云首页有非常多html结构完全一样的模块，所以决定使用react进行开发把结构相同的模块组件化，这样一来页面结构变得非常清晰并且实现了代码的复用。开发过程中发现不同的react组件之间往往需要使用对方的数据，所以使用redux来进行组件间的交流。
- 首页的轮播图部分会加载几张很大的超清图片，在网速不够快时会加载的很慢很影响体验，所以对于轮播图中的图片采用了按需加载的方式，大大提高了网页加载的速度。页面中有大量的图片，每一个图片都会发出一个请求极大的拖慢了页面的加载速度。观察发现这些图片大部分都是纯色图片，阿里巴巴矢量图标库把这些图片打包到一个字体文件中，引入该字体文件即可，大大减少了图片请求的数量。
- 适当地添加了一些css3动画使得页面的交互更加流畅、美观。
- [预览地址](https://q123321.github.io/JDcloud/build/index.html)
#### 自定义日历组件
- 一个日历组件，当我们点击input使其获得焦点时，会弹出一个日历，通过电击该日历上的按钮可以为input添加日期而不用手动输入日期。
- 利用Date函数获得当前的时间，根据时间计算出当前年、月、日，然后生成当前月的所有日子的Date对象并存入数组，然后遍历数组把当前月的日子渲染到页面中。通过事件代理的方式为这些日子添加电击事件，点击后便把对应的日期更新到input中。之后为切换月分按钮添加点击事件，切换了月份后会改变 并重新渲染当前月份的日子。
- 为了使代码更加简洁易懂，利用一个构造函数来生成日历对象，对象特有的属性通过构造函数的this在生成日历对象的时候赋予，而每一个日历对象都要用到的函数则放在构造函数的prototype对象中，这样生成的每个日历对象都能够访问到共有的函数，并且这些函数只需要声明一次就行了。
- [预览地址](https://q123321.github.io/datepicker/index.html)
#### 网页计算器
- 一个网页版的计算器应用，用户通过电击按钮输入自己想要计算的算式，按下=按钮后得到计算后的值。
- 一个算式可以拆分成很多子算式，不同的子算式计算的优先级不同，而括号中的算式优先级最高。先使用正则匹配括号中的算式，然后正则匹配括号中优先级高的子算式并计算，全部计算完之后再正则匹配优先级低一级的子算式并计算，以此类推计算出所有子算式后得到括号中的结果。把所有括号中的算式算完了后得到一个没有括号的算式，同样按照优先级从高到低计算得到结果。
- 测试时发现错误的输入会引发程序报错或者得到奇怪的结果，所以对输入的算式再计算前进行合法性校验以保证输入的算式是合法的。
- [预览地址](https://q123321.github.io/calculator/calculator.html)
#### NodeJs微信服务器
- 一个基于nodejs的koa框架开发的微信订阅号服务器程序。
- 实现了用户关注订阅号自动回复功能，实现了根据用户的输入的不同回复不同的内容功能。
- 首先要验证服务器接收到的消息是否来自微信服务器，把请求中的signature、timestamp、nonce、echostr的值读取出来，然后将token、timestamp、nonce三个参数进行字典序排序后拼接起来进行sha1加密，加密后的字符串与signature对比，若相同则该请求来自微信服务器，返回echostr。
- 对服务器传来的xml数据进行解析，解析成javascript对象，根据对象中值的不同返回不同的数据，当然返回的数据也必须按照微信开发者文档组装成xml格式数据。
## 技能评价
cs 科班毕业，对常见的数据结构和算法有一定了解。熟练使用subline和chrome开发调试工具。熟悉 W3C 规范，能熟练使用 html、css快速还原设计稿。javascript 基础扎实，对作用域、闭包、this、prototype、js的面向对象编程、promise、异步、回调等知识有着深入理解，目前正在读你不知道的javascript这本书。对 http 协议的常用状态码和缓存机制有一定了解。对前端自动化、工程化、性能优化有一定了解。框架的话比较熟悉 react、redux。对 nodejs 有一定了解，能够用express和koa框架快速搭建服务器程序。
