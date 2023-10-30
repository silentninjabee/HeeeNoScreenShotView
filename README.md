### HeeeNoScreenShotView
//translated original into english
The simplest way to disable screenshots

By chance, I discovered that when the input box is in the form of a password, neither screenshot nor screen recording can obtain the content of the input box. 
I thought that if we add our component to it, can we prohibit users from taking screenshots?
I tried it and found that it really works. 
We can remain hidden from Screen capture and screen recording at the same time.
The first subview on UITextField is _UITextFieldCanvasView. 
When it is in password mode, this view will be hidden when taking a screenshot or recording. 
So our view component is added to this view. 
Note: This method is only applicable to iOS13 and later systems. 
The demo has not been tested by the project. If there are any problems, please solve them according to the actual situation.

//Chinese Original
禁止截屏最简单的实现方法
偶然机会发现，当输入框是密码形式时，截屏和录屏都不能获取到输入框的内容，所以想到，如果把我们的组件添加到上面，是不是就可以实现禁止用户截屏了呢。
试了一下，发现真的可以，截屏和录屏一块儿搞定了。
UITextField上的第一个子view是_UITextFieldCanvasView，当是密码模式时，这个view会在截屏或者录屏时隐藏，所以我们的组件就添加在这个view上。
注意：这个方法仅适用于iOS13及以后的系统。demo没有经过项目的检验，如有问题请根据实际情况解决。

