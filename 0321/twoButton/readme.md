# Android 버튼 레이아웃

## 개요

이 프로젝트는 Android 앱에서 두 개의 버튼을 포함하는 기본적인 레이아웃을 구현합니다.

## XML 코드 (레이아웃)

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical" >

    <Button
        android:id="@+id/button1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="첫번째 버튼" />

    <Button
        android:id="@+id/button2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="두번째 버튼" />

</LinearLayout>
