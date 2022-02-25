# LengthPickerApplication


# Gradle
--------

[![jitpack][4]][5]

Add the jitpack repo to your your project's build.gradle at the end of repositories [Why?](#why-jitpack)

/build.gradle
```groovy
allprojects {
	repositories {
		jcenter()
		maven { url "https://jitpack.io" }
	}
}
```

Then add the dependency to your module's build.gradle:

/app/build.gradle
```groovy
implementation 'com.github.sunkeeper316:LengthPickerApplication:v1.0.1'
```

# How to use
--------
This is the basic usage of a single showcase view, you should check out the sample app for more advanced usage.

```java

	// single example MetricDialog
	new PickerMetricDialogFragment()
                        .setValue(m_value)
                        .setOnValueChangedListener( (view , i_value , m_value) -> {
                            
                        }).setOnOKClickListener((view, i_value, m_value) -> {
                             })
                        .show(getSupportFragmentManager(),PickerMetricDialogFragment.TAG);
                
                
                
                
	// sequence example  ImperialDialog    
    
    new PickerImperialDialogFragment()
                        .setValue(i_value)
                        .setOnValueChangedListener( (view , i_value , m_value) -> {
                            
                             })
                        .setOnOKClickListener((view, i_value, m_value) -> {
                            
                             })
                        .show(getSupportFragmentManager(),PickerImperialDialogFragment.TAG);
	
                
```