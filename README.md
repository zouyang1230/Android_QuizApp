# Android_QuizApp

## ��׿�������� ��ϰ

![APPʾ��ͼ](https://github.com/zouyang1230/Android_QuizApp/raw/master/images/Quiz.jpg)

### Tips��

1��Android SDK�����˶��������ͨ�����ø�������ɻ��������û����漰��Ϊ��ÿһ����
������View��������ࣨ��TextView��Button����һ������ʵ����

2��LinearLayout����̳���View�����ViewGroup����� 
ViewGroup����Ǹ�����������������������������������һ�л�һ�ŵ���ʽ���������ʹ��LinearLayout����Ϳ����ˡ�
����ViewGroup���໹����FrameLayout�� TableLayout��RelativeLayout��

3��AppCompatActivity�����ã���ʵ�ʾ���һ��Activity���࣬��Ҫ��ΪAndroid�ɰ汾ϵͳ�ṩ������֧�֡���13�»���ϸ����AppCompatActivity��

4��R.java����·����app/build/generated/source/r/debug

5�����Ŀ��ٵ��룺alt+enter

6�����벼�֣�
* ��activity�У���ͨ������Activity�������������ɵ������
```
public View findViewById(int id)
```

7���¼�������AndroidӦ�����ڵ��͵��¼��������͡����������л�ű������¼�������Ӧ�������󣬼���ʼ�ȴ���Ϊ�¼��ķ��������û�����ĳ����ť��

8������¼�����֮ʹ�������ڲ��ࣺ
* ����SetOnClickListener(OnClickListener)�����ļ�����������һ�������ڲ��ࣨanonymous inner class��ʵ��
```java
mTrueButton.setOnClickListener(new View.OnClickListener() {
	@Override
	public void onClick(View v) {
		// ...
	}
});
``` 

9������Toast��ʾ��Ϣ��
* ��������Toast������·������ɴ���һ��toast��
```
public static Toast makeText(Context context, int resId, int duration)
```
* �÷�����Context����ͨ����Activity��һ��ʵ����Activity�������Context�����ࣩ��
�ڶ���������toastҪ��ʾ�ַ�����Ϣ����ԴID�� Toast��������Context�����ҵ���ʹ���ַ�������ԴID������������ͨ��������Toast�����е�һ��������ָ��toast��Ϣ��ʾ�ĳ���ʱ�䡣
* ����toast�󣬿ɵ���Toast.show()��������Ļ����ʾtoast��Ϣ��