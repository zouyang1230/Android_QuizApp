# Android_QuizApp

## 安卓开发基础 练习

![APP示意图](https://github.com/zouyang1230/Android_QuizApp/raw/master/images/Quiz.jpg)

### Tips：

1、Android SDK内置了多种组件，通过配置各种组件可获得所需的用户界面及行为。每一个组
件都是View类或其子类（如TextView或Button）的一个具体实例。

2、LinearLayout组件继承自View子类的ViewGroup组件。 
ViewGroup组件是个包含并配置其他组件的特殊组件。如需以一列或一排的样式布置组件，使用LinearLayout组件就可以了。
其他ViewGroup子类还包括FrameLayout、 TableLayout和RelativeLayout。

3、AppCompatActivity的作用：它实际就是一个Activity子类，主要是为Android旧版本系统提供兼容性支持。第13章会详细介绍AppCompatActivity。

4、R.java所在路径：app/build/generated/source/r/debug

5、包的快速导入：alt+enter

6、引入布局：
* 在activity中，可通过以下Activity方法引用已生成的组件：
```
public View findViewById(int id)
```

7、事件驱动：Android应用属于典型的事件驱动类型。不像命令行或脚本程序，事件驱动型应用启动后，即开始等待行为事件的发生，如用户单击某个按钮。

8、点击事件监听之使用匿名内部类：
* 传入SetOnClickListener(OnClickListener)方法的监听器参数是一个匿名内部类（anonymous inner class）实现
```java
mTrueButton.setOnClickListener(new View.OnClickListener() {
	@Override
	public void onClick(View v) {
		// ...
	}
});
``` 

9、创建Toast提示消息：
* 调用来自Toast类的以下方法，可创建一个toast：
```
public static Toast makeText(Context context, int resId, int duration)
```
* 该方法的Context参数通常是Activity的一个实例（Activity本身就是Context的子类）。
第二个参数是toast要显示字符串消息的资源ID。 Toast类必须借助Context才能找到并使用字符串的资源ID。第三个参数通常是两个Toast常量中的一个，用来指定toast消息显示的持续时间。
* 创建toast后，可调用Toast.show()方法在屏幕上显示toast消息。