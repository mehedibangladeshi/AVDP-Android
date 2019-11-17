# AVDP-Android
All Variant DP is a Android library that can make your DP and SP values in xml files, adaptable in various screen sizes. 

- This library will handle adjustment of dp and sp values for verious screen size.   

## Adding Dependencies

Add this to at the end of repositories in project/root level build.gradle :  

```java

allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
```

add this in dependencies at app level build.gradle:

```java

dependencies {
	        implementation 'com.github.mehedibangladeshi:AVDP-Android:0.1.0'
	}
  
```

## Example

- for <b>Density Pixel</b> values Example : write `"@dimen/_24dp"` instead of `"24dp"`
- for font-size <b>SP</b> values Example: write `"@dimen/_20sp"` instead of `"20sp"`


### A code example
``` xml
<TextView
                android:id="@+id/greetings"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:gravity="center"
                android:layout_margin="@dimen/_24dp"
                android:text="Hello World"
                android:textColor="@color/colorEnamelBlue"
                android:textSize="@dimen/_22sp"
                android:textStyle="bold" />
```
