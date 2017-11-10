
Input Control=>Buttons
	
1 实现无边框按钮对应用的主题必须是Theme.Holo

2 按钮间分割线

	android:divider=“？android:dividerVertical”

  	android:dividerPadding=”8dp”
  
 	android:showDividers=”middle”
  
该三句就可在LinearLayout中实现竖直分隔线，相当于

  	Style:”?android:buttonBarStyle”(即无边框按钮间的分割线)
  
样式与主题

样式：是指为view或窗口制定外观和格式的属性集合

主题：是指对整个Activity或应用而不是对单个view应用的样式

	1 定义样式：在项目的res/values/目录中保持一个XML文件，可以通过<styles>元素的parent属性值指定继承的父类样式；自定义样式用句点进行继承的分隔
	
	2 样式属性：由<item>元素定义
	
	3 设置样式：为单个视图设置样式，为XML布局中的View元素添加style属性
	
                对整个Activity或应用设置样式，为清单文件中的<activity>或<application>元素添加android：theme属性
		
	4 根据平台版本选择主题：res/values/styles.xml，标准平台默认
							
				res/values-v11/styles.xml，API级别大于等于11的系统
							
				res/values-v21/styles.xml，API级别大于等于21的系统平台
