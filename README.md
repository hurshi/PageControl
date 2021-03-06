# ViewPager Indicators  
[![](https://jitpack.io/v/hurshi/ViewpagerIndicators.svg)](https://jitpack.io/#hurshi/ViewpagerIndicators)

viewPager indicator for Android 


### Contribute
Please do! I'm happy to review and accept pull requests.
### Developed By
* Gavin  <xujianhua.ae@gmail.com>



### Special Thanks
* Chenupt - [BezierDemo](https://github.com/chenupt/BezierDemo)


### Getting Started

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
	
	dependencies {
	        compile 'com.github.hurshi:ViewpagerIndicators:v1.0.1'
	}

##### In XML:  

	<com.e_gavin163.hsviewpageindicators.Indicator
        android:id="@+id/pagecontrol"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:layout_centerHorizontal="true"
        android:layout_marginBottom="20dp"
        android:background="@android:color/transparent"
        app:colorMovingPoint="#00ab7d"
        app:colorPoints="#545454"
        app:isFill="true" />
        
##### In Code:  

	new Indicator.Builder()
                        .setAdapter(adapter)
                        .bindViewPager(viewPager)
                        .setDefaultIndex(1)
                        .setOnPageChangeListener(new ViewPager.OnPageChangeListener()...)
			
##### All xml attributes:  

	<declare-styleable name="PageControl">
        <attr name="colorMovingPoint" format="color" />
        <attr name="colorPoints" format="color" />
        <attr name="nums" format="integer" />
        <attr name="space" format="dimension" />
        <attr name="angle" format="dimension" />
        <attr name="radiusNormal" format="dimension" />
        <attr name="radiusFocus" format="dimension" />
        <attr name="isFill" format="boolean" />
    </declare-styleable>



### Demo
![Alt Text](https://raw.githubusercontent.com/JianhuaXu/PageControl/master/demo.gif)
![Alt Text](https://raw.githubusercontent.com/JianhuaXu/PageControl/master/demo2.gif)




