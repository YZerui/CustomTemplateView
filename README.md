#CustomTemplateView 
-----
用于在客户端构建统一的UI风格，降低UI的维护难度，工程以library形式存在，可被导入到各个项目中
##有以下自定义组件可供参考使用
#####在xml布局文件中记得声明：xmlns:custom="http://schemas.android.com/apk/res-auto"
#####注：custom用于引出相关可控属性来定义视图的形式

###自定义顶部栏
	<com.customview.view.CustomTopbarView
		android:id="@+id/topBar"
		android:layout_width="fill_parent"
		android:layout_height="wrap_content"
		custom:topbar_back_text="联系人"
		custom:topbar_title="通信录" >
	</com.customview.view.CustomTopbarView>
###自定义默认界面
	<com.customview.view.CustomPageView
        android:id="@+id/pageView"
        android:layout_width="fill_parent"
        android:layout_height="fill_parent"
        android:gravity="center"
        android:visibility="gone" >
    </com.customview.view.CustomPageView>

###自定义设置栏
	<com.customview.view.CustomItemView
        android:id="@+id/activityItem"
        android:layout_width="fill_parent"
        android:layout_height="wrap_content"
        app:item_imgNote="@drawable/self_activity_note"
        app:item_splitBottomShow="SHOW"
        app:item_textContent="我的活动" />

###其它...


