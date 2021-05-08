# todo-b4a
A nice Todo List android app created using B4A

**Preview:**

<img src="https://github.com/pyhoon/todo-b4a/blob/master/Preview/1.png" width="140" title="Main" /> &nbsp; 
<img src="https://github.com/pyhoon/todo-b4a/blob/master/Preview/2.png" width="140" title="New Item" /> &nbsp; 
<img src="https://github.com/pyhoon/todo-b4a/blob/master/Preview/3.png" width="140" title="Edit Item" />

Made with ❤ in B4X

Download and Develop with B4A for **FREE**: https://www.b4x.com/b4a.html

To change the theme, add AppCompat Library and add the following lines in Manifest Editor

# Manifest Editor

``` XML
'This code will be applied to the manifest file during compilation.
'You do not need to modify it in most cases.
'See this link for for more information: https://www.b4x.com/forum/showthread.php?p=78136
AddManifestText(
<uses-sdk android:minSdkVersion="5" android:targetSdkVersion="28"/>
<supports-screens android:largeScreens="true" 
    android:normalScreens="true" 
    android:smallScreens="true" 
    android:anyDensity="true"/>)
SetApplicationAttribute(android:icon, "@drawable/icon")
SetApplicationAttribute(android:label, "$LABEL$")
'CreateResourceFromFile(Macro, Themes.LightTheme)
'End of default text.

SetApplicationAttribute(android:theme, "@style/Todo")
CreateResource(values, colors.xml,
<resources>
	<color name="actionbar">#FF8A2BE2</color>
   	<color name="statusbar">#FF8A2BE2</color>
   	<color name="navigationBar">#FF8A2BE2</color>	
   	<color name="textColorPrimary">#FF000000</color>	
   	<color name="colorAccent">#FFE91E63</color>	
</resources>
)


CreateResource(values, theme.xml,
<resources>
	<style name="Todo" parent="Theme.AppCompat.Light">
		<item name="colorPrimary">@color/actionbar</item>
        <item name="colorPrimaryDark">@color/statusbar</item>
		<item name="android:navigationBarColor">@color/navigationBar</item>		
       	<item name="android:textColorPrimary">@color/textColorPrimary</item>		
       	<item name="colorAccent">@color/colorAccent</item>
       	<item name="windowNoTitle">true</item>
       	<item name="windowActionBar">false</item>
       	<item name="windowActionModeOverlay">true</item>
    </style>
</resources>
)
```

In Main Activity, add #Extends: android.support.v7.app.AppCompatActivity
```
#Region  Activity Attributes
	#FullScreen: False
	#IncludeTitle: False
	#Extends: android.support.v7.app.AppCompatActivity
	#IgnoreWarnings: 32
#End Region
```

YouTube tutorial playlist:
https://youtube.com/playlist?list=PLnM2IRsCeAoanBmIThXgdDQpomr59iHKv
