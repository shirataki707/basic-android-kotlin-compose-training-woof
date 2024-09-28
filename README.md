Woof App
==================================
[Codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-material-theming?continue=https://developer.android.com/courses/pathways/android-basics-compose-unit-3-pathway-3?hl%3Dja%23codelab-https://developer.android.com/codelabs/basic-android-kotlin-compose-material-theming#3)

The Woof app is a list of dog photos with information about them including their name, age, and favorite activity. This app also uses Material Design to create a beautiful app experience for the user.

Screenshot
----------


Learn
-----
- Hexadecimal (Hex) Color Codes
    <!-- Add image here -->
- [Material Theme Builder](https://m3.material.io/theme-builder#/custom) が便利
- [Android StudioでMarkdownのプレビューを表示させる方法](https://qiita.com/noobar/items/8edd6f7da28666e1b5cb)
  - Dynamic Color (Material3)
    - ユーザーの壁紙に基づいてアプリのテーマを作成する
    ```kotlin
    @Composable
      fun WoofTheme(
      darkTheme: Boolean = isSystemInDarkTheme(),
      // Dynamic color is available on Android 12+
      dynamicColor: Boolean = true,
      content: @Composable () -> Unit
    ) {

- Shape
  - Composableの形状を小、中、大で定義する。
  - Cardは中サイズとして定義されている
  ```kotlin
  # Shape.kt
  val Shapes = Shapes(
    small = RoundedCornerShape(50.dp),
    medium = RoundedCornerShape(bottomStart = 16.dp, topEnd = 16.dp)
  )
  
  # Theme.kt
  MaterialTheme(
   colors = colors,
   typography = Typography,
   shapes = Shapes,
   content = content
  )
- [Fontのダウンロード](https://fonts.google.com/)
  - ダウンロードしたフォントファイルをres/fontに追加する 
  - Type.ktにフォントを追加する
- ScaffoldはスロットをTopBarなどのスロットを提供できる
  - innerPaddingを使ってTopBarなどのスロットの領域を避けてレイアウトを設定できる

Introduction
------------

This is the starter code for the Woof app project. This project is an opportunity for you to learn Material3 and reinforce the concepts you've learned so far in Android Basics with Compose.

Pre-requisites
--------------

- Rows/Columns
- Modifiers
- Scaffold
- Adding images
- Button click handlers
- Functions
- Classes
- Lists
- App architecture

Getting Started
---------------

1. Download the project
2. Open the project in Android Studio
3. Run the project
