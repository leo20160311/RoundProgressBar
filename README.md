# RoundProgressBar
一个自定义的圆形ProgressBar

##简单使用
* Step 1. Add the JitPack repository to your build file in your root build.gradle at the end of repositories:

	    allprojects {
	    	repositories {
			...
			maven { url 'https://jitpack.io' }
		    }
	    }
	
* Step 2. Add the dependency

	    dependencies {
	        implementation 'com.github.ziyexiao:RoundProgressBar:1.0.0'
	    }
	    
* step 3.在XML布局文件中添加 RoundProgressBar

          <com.xx.roundprogressbar.RoundProgressBar
                      android:id="@+id/rpb"
                      android:layout_marginTop="100dp"
                      android:layout_width="200dp"
                      android:layout_height="200dp"
                      android:layout_centerHorizontal="true"
                      app:secondTextSize="45sp"
                      app:thirdText="kg"
                      app:topText="体重"
                      app:topTextSize="16sp"
                      app:animationDuration="1500"
                      app:progressArgbColor="true"
                      app:thirdTextSize="16sp" />
                    
* step 4.添加代码

         RoundProgressBar rpb = findViewById(R.id.rpb);
         //设置当前进度
         rpb.setCurrentProgress(100);
         //设置最大进度
         rpb.setMaxProgress(100);
         
###效果图
![效果图](http://m.qpic.cn/psb?/V14Ej48r2rOT1E/xF3UHkspNPUm4kCY70ABO3leri2yTmKguFV0d2VvafE!/b/dFkAAAAAAAAA&bo=aAGAAmgBgAICOR0!&rf=viewer_4)

##参数说明

>1. **argbColor**：是否进行颜色渐变变化（如果设置为true的话，则文字颜色与进度条颜色都会设置无效）
>2. **topText**：第一行文本
>3. **topTextSize**：第一行文本大小
>4. **secondTextSize**：中间文本文本大小（进度大小）
>5. **thirdText**：第三行文本
>6. **thirdTextSize**：第三行文本大小
>7. **animationDuration**：修改当前进度后执行的动画时长
>8. **currentProgress**：当前进度
>9. **maxProgress**：最大进度
>10. **circleColor**：圆环底色
>11. **circleThickness**：圆环宽度
>12. **progressStartColor**：圆弧渐变开始颜色
>13. **progressEndColor**：圆弧渐变结束颜色


       
        
 
 

