# NativeFlutterProject
一个简单的iOS工程，用于Flutter混合开发。实现了
- iOS端业务开发者无需安装Flutter开发环境，可以方便快捷的引入Flutter业务内容。
- Flutter业务开发者可以方便的attach到Native工程进行原生应该环境下的Flutter开发。

相关细节介绍：
- Flutter工程开发Flutter业务后编译产物使用pod私有库方式引入到iOS工程。[Flutter工程地址](https://github.com/X-HH/FlutterProject)
- iOS工程引入flutter_boost，进行Fluuter页面栈的管理。主要的衔接工具类是XHFlutterRouter。
- Flutter与iOS原生的相互调用，Flutter调用原生方法的意义是可以调用原生的能力和数据传递，原生调用Flutter的意义是原生可以控制Flutter的表现。

总结：

该工程主要意义在于提供了一套iOS原生与Flutter混合编程的整体解决方案。基本抹平了在混合开发中的几个重要需求：

1. iOS与Flutter开发者相互隔离，
2. iOS与Flutter能力的相互调用与数据传递
3. 使用pod管理代码引入，可以很好的进行版本控制

当然了，实际的生产环境的工程运用还需要补足各种细节跟实际需求所需的相关改造。

工程运行效果：

![](https://xhhimages.oss-cn-beijing.aliyuncs.com/222.gif?Expires=1585550173&OSSAccessKeyId=TMP.3Kg1xD8E7ihRFmuKwAjwfgMyiThYJ4t3yo8wHjDkLcuLGR5oLghAtYf1Cu23zQrocFzATj6D9uRQr2JnSaAoeCdbj3R1r8&Signature=%2F2naGkEau4tES3m0vyQgPpKO8M8%3D)
