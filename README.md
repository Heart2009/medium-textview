# medium-textview
Medium android application display content with text, image, video etc in post detail. It can me a pain to do it with content came from CMS. So i decided to design that View to display the content quickly

#Screenshot
![Screenshot](https://github.com/angebagui/medium-textview/blob/master/screenshot/Screenshot_2016-08-14-19-59-48.png)


Download
========

In your dependences
```groovy
repositories {
    maven {
        url 'https://dl.bintray.com/angebagui/maven/'
    }
}

dependencies {
  compile 'io.github.angebagui.mediumtextview:mediumtextview:1.0.0'
}
```
#Usage
In my layout xml
```xml
    <ScrollView
        android:layout_width="match_parent"
        android:layout_height="match_parent">
        <io.github.angebagui.mediumtextview.MediumTextView
            android:id="@+id/medium_text_view"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="@dimen/activity_horizontal_margin"
            android:layout_marginBottom="@dimen/activity_vertical_margin"
            />
    </ScrollView>
```
Now in java code we add set the content now
```java
        MediumTextView mediumTextView = (MediumTextView)findViewById(R.id.medium_text_view);
        mediumTextView.setText(getContentHtml());
```

Licences
=======
    Copyright 2016 Ange Bagui.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
