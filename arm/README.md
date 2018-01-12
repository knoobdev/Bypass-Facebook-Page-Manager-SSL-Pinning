# Bypass Facebook Page Manager SSL Pinning (REQUIRE ROOTED)
Bypassing Facebook SSL pinning for version 145.0.0.22.381 | arm | January 11, 2018
[Download Link](https://www.apkmirror.com/apk/facebook-2/pages-manager/pages-manager-145-0-0-22-381-release/facebook-pages-manager-145-0-0-22-381-2-android-apk-download/)


#### libcoldstart.so

Replace the libcoldstart.so file in **/data/data/com.facebook.pages.app/lib-xzs**



## Steps:



We need to patch **0x0028E974** and **0x0028E976**:

![before_patching](https://raw.githubusercontent.com/knoobdev/Bypass-Facebook-Page-Manager-SSL-Pinning/master/arm/before_patch.jpg?54119)


After patching these offsets to **0xB1C4** and **0xB948**, patched lib should be like this:


![after_patching](https://raw.githubusercontent.com/knoobdev/Bypass-Facebook-Page-Manager-SSL-Pinning/master/arm/after_patch.jpg?54119)

---



[Refrence](https://serializethoughts.com/2016/08/18/bypassing-ssl-pinning-in-android-applications/) & Thanks for [pouyadarabi](https://github.com/pouyadarabi/Facebook_SSL_Pinning)

