安装某些高特性插件的时候会需要到java8支持，例如`react-native-video`


在 `/android/app/build.gradle` 添加以下代码

```gradle
android {
  ...
  defaultConfig {
    ...
    multiDexEnabled true

  }
  ...
  compileOptions {
      sourceCompatibility JavaVersion.VERSION_1_8
      targetCompatibility JavaVersion.VERSION_1_8
  }
}
```
