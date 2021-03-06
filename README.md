# ZKReactSummary
总结关于React的知识, 主要是对react文档的一些翻译以及redux, react-native的一些总结

### （一）教程

1. 笔者翻译了一篇关于 [React的思想](translation/README.md) 的文章, 翻译自英文文档.
2. 刘一奇老师的相关资料
    * [React+Redux系列教程](https://github.com/lewis617/react-redux-tutorial)
    * GitBook [Redux中文翻译](http://cn.redux.js.org/docs/introduction/Motivation.html)
3. 阮一峰老师的 [React全栈工程师培训教程](http://www.ruanyifeng.com/blog/2016/11/javascript.html) <br />
    * Redux三部曲
        1. [Redux 入门教程（一）：基本用法](http://www.ruanyifeng.com/blog/2016/09/redux_tutorial_part_one_basic_usages.html)
        2. [Redux 入门教程（二）：中间件与异步操作](http://www.ruanyifeng.com/blog/2016/09/redux_tutorial_part_two_async_operations.html)
        3. [Redux 入门教程（三）：React-Redux 的用法](http://www.ruanyifeng.com/blog/2016/09/redux_tutorial_part_three_react-redux.html)
    * 阮一峰老师的 [技术栈系列教程](http://www.ruanyifeng.com/blog/2016/09/react-technology-stack.html)
4. 深入浅出的比较好的redux教程, [地址传送带](https://github.com/kenberkeley/redux-simple-tutorial)
    * [简明教程](https://github.com/kenberkeley/redux-simple-tutorial)
    * [进阶教程](https://github.com/kenberkeley/redux-simple-tutorial/blob/master/redux-advanced-tutorial.md)
5. xujinyang的 [总结列表](https://github.com/xujinyang/react-native-android-guide) (里面有redux等相关内容)
6. LeoMobileDeveloper的 [总结列表](https://github.com/LeoMobileDeveloper/ReactNativeMaterials)
7. 一篇该概括比较全的博文 [关于 React Native，您想知道的都在这里了](https://my.oschina.net/osccreate/blog/778348)
8. [高质量的React相关文档和翻译](https://github.com/react-guide)
    * [React设计思想](https://github.com/react-guide/react-basic)
    * [Redux教程](https://github.com/react-guide/redux-tutorial-cn#redux-tutorial)
    * [Redux中文文档](https://github.com/camsong/redux-in-chinese)
9. 知乎上关于 react 的话题:
    * 阿里的陈屹大大主创的知乎专栏 [pure render](https://zhuanlan.zhihu.com/purerender) 干货满满, 推荐多研究研究.  
        * 陈屹老师的心血之作[《深入react技术栈》](https://zhuanlan.zhihu.com/p/22516062?refer=purerender)中的实例源码 [react-book-examples](https://github.com/arcthur/react-book-examples)  
    * [理解 React，但不理解 Redux，该如何通俗易懂的理解 Redux？](https://www.zhihu.com/question/41312576)
    * [看漫画，学 Redux](https://github.com/jasonslyvia/a-cartoon-intro-to-redux-cn)

### （二）实例

1. 一篇比较好理解的 [TodoListDemo](https://github.com/TongchengQiu/TodoList-as-redux-demo)
2. 基于 react + react-router + redux + webpack + ES6 + less 的完整项目, 对`React`和`Redux`, `Router`也解释的比较全, 
    地址在 [这里](https://github.com/bailicangdu/react-pxq)
3. 非常好的具有文字展示和评论功能的社区软件, 基于webpack + react + react-router + redux + less + flex.css + ES6 的React版cnode社区, [传送门](https://github.com/lzxb/react-cnode)
4. 极简的 [Redux实例](./examples/simple-redux)

### （三）语法

1. 关于ES6的语法
    * 阮一峰老师的开源书[ES6标准入门(第二版)] (http://es6.ruanyifeng.com/#docs/intro) , 感谢阮大大的开源精神.
    * 大名鼎鼎的JS高程设计作者Zakas老师也开源了ES6的语法书籍, [Understanding ECMAScript 6](https://leanpub.com/understandinges6/read)
    本书的介绍的git地址在 [这里](https://github.com/nzakas/understandinges6), 
    当然, 你可以看 [中文译文](https://www.gitbook.com/book/oshotokill/understandinges6-simplified-chinese/details) , 感谢译者.
2. 阮一峰老师推荐的一个语法规范的小册子, 有正反两个实例, 非常值得阅读. [语法简洁之道](https://github.com/ryanmcdermott/clean-code-javascript)
3. babel 提供的 ES6/ES7 转 ES5 的网站, 不错值得分享. [传送门](http://babeljs.io/repl/) 

### （四）其他

1. 关于 Web 前端的性能问题
    * 存在的问题:如下
    阮一峰老师的 [也许, DOM 不是答案](http://www.ruanyifeng.com/blog/2015/02/future-of-dom.html) 提到 web 前端的性能问题  
       >
       Web app的性能瓶颈，主要有以下原因。  
         （1）Web基于DOM，而DOM很慢。浏览器打开网页时，需要解析文档，在内存中生成DOM结构，如果遇到复杂的文档，这个过程是很慢的。可以想象一下，如果网页上有上万个、甚至几十万个形状（不管是图片或CSS），生成DOM需要多久？更不要提与其中某一个形状互动了。  
         （2）DOM拖慢JavaScript。所有的DOM操作都是同步的，会堵塞浏览器。JavaScript操作DOM时，必须等前一个操作结束，才能执行后一个操作。只要一个操作有卡顿，整个网页就会短暂失去响应。浏览器重绘网页的频率是60FPS（即16毫秒/帧），JavaScript做不到在16毫秒内完成DOM操作，因此产生了跳帧。用户体验上的不流畅、不连贯就源于此。  
         （3）网页是单线程的。现在的浏览器对于每个网页，只用一个线程处理。所有工作都在这一个线程上完成，包括布局、渲染、JavaScript执行、图像解码等等，怎么可能不慢？  
         （4）网页没有硬件加速。网页都是由CPU处理的，没用GPU进行图形加速。  
         上面这些原因，对于PC还不至于造成严重的性能问题，但是手机的硬件资源相对有限，用户互动又相对频繁，结果跟Native app一比，就完全落在了下风。  
       
    * 解决方案:
        1. FlipBoard 的解决方案 [react-canvas](https://github.com/Flipboard/react-canvas)  
        具体实现详见 [60 FPS ON THE MOBILE WEB](http://engineering.flipboard.com/2015/02/mobile-web/)  
        [中文译文](https://zhuanlan.zhihu.com/p/19967854)
        
2. [TypeScript 教程](https://github.com/xcatliu/typescript-tutorial)
