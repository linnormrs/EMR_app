# emr_app

arduino's EMR data visulaization app

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.


### Design Link
- [figma design link](https://www.figma.com/file/tdCQgx1XSx485wXv7L1K0k/OOP_EMR_APP?node-id=9%3A2)



### 개인적 공부
##### [플러터 프로젝트 폴더의 구성]
> lib
>> - flutter 앱의 소스가 작성된 main.dart 파일  
>> - 당장은 여기에 집중하면 될듯

> android
>> 운영체제에서 프로젝트를 시작할 때 필요한 파일  

> ios  
>> 운영체제에서 프로젝트를 시작할 때 필요한 파일

> test
>> 다트 코드로 함수를 테스트할 때 사용하는 파일  
>> *일반적으로 함수를 테스트하려면 앱을 다시 실행해야해서 시간이 걸리는데, 플러터 프로젝트는 test를 통해 편리하게 테스트 가능


> root
>> pubspec.yaml
>>> - 다양ㅏㄴ 패키지와 이미지, 폰트 등을 사용할 수 있게 해줌


##### main.dart

**[import]**

<code>
import 'package:flutter/material.dart';
</code>

- 사용하려는 패키지를 불러올 때 사용하는 구문
- 다른 dart calss나 pubspec.yaml에서 내려받은 패키지를 불러오기 위해서도 사용

**[main()]**

<code>
void main() {
  runApp(const MyApp());
}
</code>

- dart app은 main.dart의 main()함수부터 시작

- rupApp()함수를 호출
    - binding.dart 클래스에서 정의되어, 플러터 앱을 시작하는 역할
    - 앱을 시작하면서 화면에 표시할 위젝을 전달된다.
    - tutorial에서는 MyApp이 전달된다.



**[MyApp class]**

<code>
class MyApp extends StatelessWidget {
  const MyApp({super.key});
application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      theme: ThemeData(
      home: const MyHomePage(title: 'Flutter Demo Home Page'),
    );
  }
}
</code>

- main()의 runApp()으로 플러터 앱을 실행할 때 화면에 표시할 위젝으로 전달한 MyApp 클래스를 정의

- extends: 상속 
    - Stateless Widget: tkdxork qusrudehlwl dksgsms dnlwpt

- @override, build
    - 어떠한 위젯을 만들것인지 정의
    - MaterialApp()
        - title: doqdml dlfma
        - theme: 앱의 테마의 색상
            - primarySwatch: Colors.blue
            - visualDensity: 앱이 모바일, 웹, 데스크톱, 맥 등 어떤 ㅒㄴdptjeh wkdustmfjqrp qhdlehfhr wldnjs
        - home: 첫화면에어떤 내용을 표시할지 정의


