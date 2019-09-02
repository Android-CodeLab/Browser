# Jamun-Browser

Browser Library provide you two type of In-APP Browser Functionality with Event Handling and Functions to Customize Views. 

1. `Single Pager` allow you to create Single Page In-App-Browser with custom functions and Event Hanlding Approaches.

2. `Multi Pager` allow you to create Multi Page In-App-Browser  with custom functions and Event Hanlding Approaches.

### What's New? {Latest Version}
* Stable official Version for Rapid Development.
* Custom UI components with Single and Multi Pager Mode.
* Easy Calling mechanism with instant reply via Listeners and custom functions support
* All the views in the library are Screen compatible i.e. You can execute this library on different android screens including tabs.

### Quality Measures? for {Latest Version}

The following apps are using this library without facing any kind of Bugs.

* **[SimplyBlood](https://play.google.com/store/apps/details?id=com.simplyblood)**
* **[ZINI](https://play.google.com/store/apps/details?id=ai.zini)**,
* **[RentalBazar](https://play.google.com/store/apps/details?id=com.rentalbazaar)** 
* **[DoubtCrusher](https://play.google.com/store/apps/details?id=com.doubtcrusher)**
* **[BookAGround](https://play.google.com/store/apps/details?id=com.bookaground)**
* **[PeyFree](https://play.google.com/store/apps/details?id=com.peyfree)**
* **[ClueRace](https://play.google.com/store/apps/details?id=com.cluerace)**
* **[QR/Barcode Scanner](https://play.google.com/store/apps/details?id=com.scanner.android)** 
* **[Wall-E](https://play.google.com/store/apps/details?id=com.walle.android)**
* **[CIS-Connect In Single](https://play.google.com/store/apps/details?id=com.connectinsingle)**

------
# Why this library?

* This library competible with all screen sizes and device (Tab with 7' inches and 10'inches).
* Library support both orientation that is portrait and landscape.
* Its simple and easy to use.
* Its Customizable (Support Custom Themes). 
* Minimum API is 15, but it'll probably work in API 9 and above, just make sure you test it out (we use `Support Fragment Manager`).  

### All-in-One Setup

The easiest way to add **Browser** library to your project is by adding it as a dependency to your `build.gradle`. To add picker library you just need to append few lines into your `build.gradle`.
These lines are provided in Integration Part given Below

### Gradle Configuration

**Add the dependency**

Step 1\. Add the jCenter repository to your build file. Add it in your root build.gradle at the end of repositories:

```
allprojects {
  repositories {
        mavenCentral()
  }
}
```
Step 2\. Add the dependency
```
Latest Version : 0.0.8

Android
dependencies {
     compile 'tk.jamun.ui:browser:{Latest Version}'
}

AndroidX
dependencies {
     compile 'tk.jamunx.ui:browser:{Latest Version}'
}

Kotlin
dependencies {
     compile 'tk.jamun-ktx.ui:browser:{Latest Version}'
}
```

### Maven Config

```xml
<dependency>
Android
  <groupId>tk.jamun.ui</groupId>
AndroidX
  <groupId>tk.jamunx.ui</groupId>
Kotlin
  <groupId>tk.jamun-ktx.ui</groupId>
  <artifactId>browser</artifactId>
 <version>{Latest Version}</version>
  <type>aar</type>
</dependency>
```
------

# Types of Pickers

## Single Page Browser

`Singlel Page Browser` consist of Single Pager Browser Functionality with methods calls to customize view properties and listener events to handle click events with Current Url.

#### Gradle Setup

Step 1\. Add the jCenter repository to your build file. Add it in your root build.gradle at the end of repositories:

```java
allprojects {
  repositories {
        mavenCentral()
  }
}
```
Step 2\. Add the dependency

```java

Latest Version : 0.0.8

Android
dependencies {
     compile 'tk.jamun.ui:singlepagebrowser:{Latest Version}'
}

AndroidX
dependencies {
     compile 'tk.jamunx.ui:singlepagebrowser:{Latest Version}'
}

Kotlin
dependencies {
     compile 'tk.jamun-ktx.ui:singlepagebrowser:{Latest Version}'
}
```
#### Maven
```xml
<dependency>
 Android
  <groupId>tk.jamun.ui</groupId>
AndroidX
  <groupId>tk.jamunx.ui</groupId>
Kotlin
  <groupId>tk.jamun-ktx.ui</groupId>
  <artifactId>singlepagebrowser</artifactId>
  <version>0.0.2</version>
  <type>aar</type>
</dependency>
```

Single Page Browser | Options
---- | ----
![Jamun-Single-Page-Browser-Options](https://user-images.githubusercontent.com/38988514/64109990-81ef9600-cd9e-11e9-9b38-a68e4f652d17.png) | ![Jamun-Single-Page-Browser](https://user-images.githubusercontent.com/38988514/64109992-81ef9600-cd9e-11e9-93f3-0aecd34c1d78.png)



## Multi Page Browser

`Multi Page Browser` consist of Single Pager Browser Functionality with methods calls to customize view properties and listener events to handle click events with Current Url.
l
#### Gradle Setup

Step 1\. Add the jCenter repository to your build file. Add it in your root build.gradle at the end of repositories:

```java
allprojects {
  repositories {
        mavenCentral()
  }
}
```
Step 2\. Add the dependency

```java
Latest Version : 0.0.8

Android
dependencies {
     compile 'tk.jamun.ui:mulitpagebrowser:{Latest Version}'
}

AndroidX
dependencies {
     compile 'tk.jamunx.ui:mulitpagebrowser:{Latest Version}'
}

Kotlin
dependencies {
     compile 'tk.jamun-ktx.ui:mulitpagebrowser:{Latest Version}'
}

```
#### Maven
```xml
<dependency>
  Android
  <groupId>tk.jamun.ui</groupId>
AndroidX
  <groupId>tk.jamunx.ui</groupId>
Kotlin
  <groupId>tk.jamun-ktx.ui</groupId>
  <artifactId>mulitpagebrowser</artifactId>
  <version>0.0.2</version>
  <type>aar</type>
</dependency>
```
------

# How to Implement

Once the project has been added to gradle, You can use these lines of code to configure pickers....

## 1. Single Page Browser

```
new SinglePageBrowser().setOnClickListener(new Browser.OnClickListener() {
            @Override
            public void onClickOptionMenu(int eventId, String currentUrl) {
            }
        }).startActivity(this, "https://github.com/Lib-Jamun/Browser");

```
------

## 2. Multi Page Browser

```

```


## 3. Additional Options

**1. **Share Picker Setup Details**

```
singlePageBrowser.setShareSubject("Email SUbject","Share Description with Url");
singlePageBrowser.setDisableJavascript(false);
singlePageBrowser.setToastMessageUrlCopied("Copied to Clipboard Successfully");
singlePageBrowser.setCopyToClipboardTitle("Library");
singlePageBrowser.setBoundUrlToHost(true); 
```

**2. **ClipBoard Setup Details**

```
singlePageBrowser.setToastMessageUrlCopied("Copied to Clipboard Successfully");
singlePageBrowser.setCopyToClipboardTitle("Library");
```

**3. **Disable JavaScript**

```
singlePageBrowser.setDisableJavascript(false);
```
**4. **Disable Zoom Functionality**

```
singlePageBrowser.setBuiltInZoomControls(boolean);
singlePageBrowser.setDisplayZoomControls(boolean);
```

**5. **Bound Url Setup Details**

```
singlePageBrowser.setBoundUrlToHost(true); 
```
**6. **Scrolling Bar Functionality**

```
singlePageBrowser.setVerticalScrollBarEnabled(boolean);
singlePageBrowser.setHorizontalScrollBarEnabled(boolean);
```

**7. **Set Multi Window Functionality**

```
singlePageBrowser.setSupportMultipleWindows(boolean);
```

## 3. Critical Note

**Progaurd Editing**

```
-keep class org.jsoup.**
```

> **To understand more how the library works, please take a look at the sample app.**

------

# Dependency

* Org.Jsoup Lib for URL meta parsing

## Credits

Desgin & Developed by : **[Jatin Sahgal](https://www.linkedin.com/in/jatinsahgal/)**
 (**[Linkedin](https://www.linkedin.com/in/jatinsahgal/)** & **[Website](http://androidcodelab.com/)** & **[Github](https://github.com/Lib-Jamun)**) 

## More Library under Jamun

* **[Pickers](https://github.com/Lib-Jamun/Pickers.git)**
Pickers Library provide you a set of Pickers like Country, Language, Share and Intent Chooser.

* **[Country-Pickers](https://github.com/Lib-Jamun/Pickers.git)**
allow you to access Country picking functionality with great UI/UX design, and there are numberous of function which help you to modify picker as per your requirements. Library has been provided with four custom UI initate mode you can decide how the view of picker can be initate. You can also decide weather picker inheriate Single or Multi Selection property. Library consists of updated collection of country name, code and there flags. We are using APIs base structure to avoid increase in the size of apk due to flag Images. This module Maintain the database so that you don't need to call APIs again and again rather than you can choose when to refresh the Database and fetch new real time data.

* **[Language-Pickers](https://github.com/Lib-Jamun/Pickers.git)**
provides you read-made Language picker  which is easy to use and comes with great UI/UX, and there are numberous of function which help you to modify picker as per your requirements. Library has been provided with four custom UI initate mode you can decide how the view of picker can be initate. You can also decide weather picker inheriate Single or Multi Selection property.

* **[Share-Dialog-Pickers](https://github.com/Lib-Jamun/Pickers.git)**
provide you Intent Chooser with great UI/UX. It automatically retrive the sort list of all the apps which can share the file. This functionality saves much of your task. You can also share dialog Picker for sending Large files. For this you just need to call a single function with file as Argument.
* **[Volley](https://github.com/Lib-Jamun/Volley.git)**
Library is a set of Custom Classes with UI components for network programming, integration and transaction handling in a better and standard way. This will help developers for making quality use of volley library. 

* **[Scanner](https://github.com/Lib-Jamun/scanner.git)** is a collection of Beautiful Activity which help others to make there own Custom QR/Barcode Scanner. 

* **[Calendar](https://github.com/Lib-Jamun/calendar.git)**
is a collection of Beautiful Activities which help others to make there Fully Custom Calendar View with Single and Multi Date Picker Functionality 

* **[Camera](https://github.com/Lib-Jamun/Camera.git)**
library provide you Custom Complete Camera view with full features like Flash, Rotation, Gallery Picker, Focus, Tap to capture, Confirmation window and last but not least croping feature. It also provide you file path in return so that developer can feel a friendly handy way to Deal After. 

* **[Gallery](https://github.com/Lib-Jamun/Gallery.git)**
have some Beautiful UI Components and Multi files Mode for android Developers to give there app a A Rich look With single and Multi picker Functionality.

* **[UI](https://github.com/Lib-Jamun/ui.git)**
library is a set of UI Views, Custom Component and Collection of Helper Classes which help Developer for making quality Product. Such as Camera, Gallery, Number of Pickers, Calendar, Date Pickers, Dialogs and many more Heler UI and Backend Component.

## License
    Copyright (c) 2018 Jatin Sahgal

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
