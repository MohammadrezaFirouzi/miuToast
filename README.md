# MiuToast


[![platform](https://img.shields.io/badge/platform-Android-yellow.svg)](https://www.android.com)
 [![API](https://img.shields.io/badge/API-21%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=21)
 


![MiuToast](https://uploadkon.ir/uploads/613308_24images.jpg)

**A material design Toast Library for Android**



## Screenshots


![Screenshot](https://uploadkon.ir/uploads/ec2008_24InShot-20240408-191655664.jpg)


## Prerequisites

Add it in your root build.gradle at the end of repositories:

```gradle
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
        repositories {
            mavenCentral()
            maven { url 'https://jitpack.io' }
	}
}
```
<br/>

## Dependencies

Add this to your module's `build.gradle` file (make sure the version matches the JitPack badge above):

```gradle
dependencies {
    implementation 'com.github.MohammadrezaFirouzi:MiuToast:Tag'
}
```
<br/>


## Usage

Each of the following method returns a `Toast`. **Don't Forget to Call `.show()`**

To display an Info Toast:

``` java
       CuteToast.ct(this, "This is a Info Toast", CuteToast.LENGTH_SHORT, CuteToast.INFO, true).show();
```
To display a Warning Toast:

``` java
       CuteToast.ct(this, "This is a Warning Toast", CuteToast.LENGTH_SHORT, CuteToast.WARN, true).show();
```
To display an Error Toast:

``` java
       CuteToast.ct(this, "This is a Error Toast", CuteToast.LENGTH_SHORT, CuteToast.ERROR, true).show();
```
To display a Success Toast:

``` java
       CuteToast.ct(this, "This is a Success Toast", CuteToast.LENGTH_SHORT, CuteToast.SUCCESS, true).show();
```
To display a Happy Toast:

``` java
       CuteToast.ct(this, "This is a Happy Toast", CuteToast.LENGTH_SHORT, CuteToast.HAPPY, true).show();
```
To display a Sad Toast:

``` java
       CuteToast.ct(this, "This is a Sad Toast", CuteToast.LENGTH_SHORT, CuteToast.SAD, true).show();
```
To display a Confuse Toast:

``` java
       CuteToast.ct(this, "This is a Confuse Toast", CuteToast.LENGTH_SHORT, CuteToast.CONFUSE, true).show();
```
To display a Delete Toast:

``` java
       CuteToast.ct(this, "This is a Delete Toast", CuteToast.LENGTH_SHORT, CuteToast.DELETE, true).show();
```
To display a Save Toast:

``` java
       CuteToast.ct(this, "This is a Save Toast", CuteToast.LENGTH_SHORT, CuteToast.SAVE, true).show();
```
To display a Normal Toast:

``` java
       CuteToast.ct(this, "This is a Normal Toast", CuteToast.LENGTH_SHORT, CuteToast.NORMAL, true).show();
```

<br/>

### If you don't want the Icons:
#### Replace `true` to `false` at the end of the statment.

``` java
       CuteToast.ct(this, "This is a Info Toast", CuteToast.LENGTH_SHORT, CuteToast.INFO, false).show();
```

``` java
       CuteToast.ct(this, "This is a Error Toast", CuteToast.LENGTH_SHORT, CuteToast.ERROR, false).show();
```

and same for the other types too. 

#### Or Just Remove the last `boolean` part

``` java
       CuteToast.ct(this, "This is a Info Toast", CuteToast.LENGTH_SHORT, CuteToast.INFO).show();
```

``` java
       CuteToast.ct(this, "This is a Error Toast", CuteToast.LENGTH_SHORT, CuteToast.ERROR).show();
```

<br/>

### If you want to use Custom Icons:

``` java
        CuteToast.ct(this, "This is an Info Toast with Custom Star Icon", CuteToast.LENGTH_SHORT, CuteToast.INFO, R.drawable.ic_star).show();
```

``` java
        CuteToast.ct(this, "This is an Error Toast with Custom Danger Icon", CuteToast.LENGTH_SHORT, CuteToast.ERROR, R.drawable.danger_ic).show();
```

## Notes


* If `this` shows an error, then replace it with `MyActivity.this` where MyActivity is your activity name.
* Durations are `CuteToast.LENGTH_SHORT` and `CuteToast.LENGTH_LONG` .
* Total 10 Background Desings are available:
	- INFO
	- WARN
	- ERROR
	- SUCCESS
	- HAPPY
	- SAD
	- CONFUSE
	- DELETE
	- SAVE
	- NORMAL
* Icon Options:
	- If `icon` is `true`, then pre-built icons will be shown
	- If 'icon` is 'false` or 'boolean' is removed, then no icon will be shown
	- If 'icon' is added by using `R.drawabale.icon_name` , then custom icon will be shown.
* If you use the Custom Dependency (`implementation 'com.github.ahmmedrejowan.CuteToast:CuteToast-Custom:1.1`) then you can't use the pre-built icons.



<br/>


## Contribute

Please fork this repository and contribute back using [pull requests](https://github.com/ahmmedrejowan/CuteToast/pulls).

Any contributions, large or small, major features, bug fixes, are welcomed and appreciated
but will be thoroughly reviewed .

Let me know which features you want in the future in `Request Feature` tab. 

If this project helps you a little bit, then give a to Star ⭐ the Repo. 

<br/>


## Credits

Created with Love by **K M Rejowan Ahmmed** (@ahmmedrejowan)

Reach me @
* [Github](https://github.com/ahmmedrejowan) 
* [LinkedIn](https://www.linkedin.com/in/ahmmedrejowan)
* [Twitter](https://twitter.com/ahmmedrejowan)
* [Facebook](https://facebook.com/ahmmedrejowan)
* [StackOverFlow](https://stackoverflow.com/users/9932194/k-m-rejowan-ahmmed)




## License

* [Apache Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

```
Copyright 2021 K M Rejowan Ahmmed (ahmmedrejowan)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

```




