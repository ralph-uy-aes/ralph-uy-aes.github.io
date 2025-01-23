---
layout: project
type: project
image: img/Medex/logo.jpg
title: "MedEx"
date: 2020
published: true
labels:
  - Android App
  - Java
  - Android Studio
  - Medicine
  - Ecommerce
summary: "A group of friends and I decided to try to solve the issue of delivering pharmaceutical supplies to Filipino citizens during the COVID-19 pandemic."
---

<div class="text-center p-4">
  <img width="550px" src="../img/Medex/inventory.png" class="img-thumbnail" >
</div>

MedEx was a delivery app that never got released. What primarily distinguished it from other delivery apps at the time was its novel focus on pharmaceutical supplies such as rubbing alcohol, prescription medicine, health supplements, vitamins, and more. Back in 2020, this was not very common mainly because of the pandemic, but also, during this time, online food delivery through mobile applications was only an emerging industry. Another thing that distinguished this project was how young the members of the group were. We had an older friend who knew more about software engineering more than us and he acted as our consultant during this project. I believe I was the youngest in the group being only 14 or 15 years old. My peers were a year older than me.

The reason for the conception of this app was the strict lockdown implemented by the government during the time of the COVID-19 pandemic. Naturally, it would have been quite difficult for people to go outside and buy their necessities from pharmacies. So, why not expand on an emerging market?

For this project, I was the UI/UX designer, meaning I mostly worked on the front end. I designed various custom-made UI elements such as containers for products, product pages, home page designs, and more. I used android studio's built-in containers and overlayed my own graphics onto them. I also began creating the database for the products using firebase.

We never got to finish this project due to lockdown restrictions being lifted and because we had a lot of schoolwork at the time.

This is the android manifest of MedEx.
```cpp
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.empiricus.medex">

    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
    <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />


    <application
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="MedEx"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme"
        android:hardwareAccelerated="true">
        <activity android:name=".main.SignIn">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
        <activity android:name=".main.SignUp"> </activity>
        <activity android:name=".main.ForgotPassword" > </activity>
        <activity android:name=".main.Home"> </activity>
        <activity android:name=".main.ItemMain"/>
        <activity android:name=".main.DriverSignIn" />
        <activity android:name=".main.DriverSignUp"/>
        <activity android:name=".main.DriverSignUp2"/>
        <activity android:name=".main.DriverSignUp3"/>
        <activity android:name=".main.MerchantSignIn"/>
        <activity android:name=".main.MerchantHome"/>
        <activity android:name=".main.MerchantSignUp"/>
        <activity android:name=".main.MerchantSignUp2"/>
        <activity android:name=".main.Checkout"/>
        <activity android:name=".main.MerchantSignUp3"/>
        <activity android:name=".main.OnBoarding"> </activity>

        <service
            android:name="com.empiricus.medex.fragments.FetchAddressIntentService"
            android:enabled="true" />

        <meta-data
            android:name="com.google.android.geo.API_KEY"
            android:value="AIzaSyBZPTiJOwLbqyUVQzwf3IOh4S0zGeVuYdo" />

    </application>

    <uses-feature
        android:glEsVersion="0x00020000"
        android:required="true" />

</manifest>
```
