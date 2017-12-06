Chosun-OSS
====================

조선대학교 오픈 소스 소프트웨어 프로젝트 입니다.

02분반 11조 조장 조태호.

*상세한 GitHub 히스토리는 GitHub_History.pdf 문서에 첨부하였습니다.*

## 프로젝트 목차

1. [Android Signature Pad](#android-signature-pad)
 * README.md 번역
 * 오픈 소스 프로젝트에 기능을 추가하여 릴리즈

2. [Cordova GoogleMaps Plugin](#cordova-googlemaps-plugin)
 * README.md 번역

3. [HTTP JSON](#http-json)
 * 신규 오픈소스
 * JAVA 라이브러리 오픈 소스 개발

## Android Signature Pad

안드로이드에서 터치를 통해 필기 서명(Signature)을 할 수 있도록 하는 라이브러리입니다.

원본 프로젝트인 [gcacace/android-signaturepad](https://github.com/gcacace/android-signaturepad)를 Fork 하여, [setreuid/android-signaturepad](https://github.com/setreuid/android-signaturepad)에서 README.md 한글화 하였습니다.

추가로, 이 라이브러리를 사용하던 중에 불편했던 [웹에서 기존 서명 이미지를 바로 불러오는 기능](https://github.com/setreuid/android-signaturepad/commit/02188883010972d4d330c215b896520b1120eac3)을 추가하여
[버전 1.2.1.1](https://github.com/setreuid/android-signaturepad/releases/tag/1.2.1.1)을 릴리즈하고 JitPack을 통해 배포하고 있습니다.

## Cordova GoogleMaps Plugin

하이브리드 앱 개발시 네이티브 구글 맵 SDK를 연동해주는 Cordova 플러그인입니다.

원본 프로젝트인 [mapsplugin/cordova-plugin-googlemaps](https://github.com/mapsplugin/cordova-plugin-googlemaps)를 Fork 하여, [setreuid/cordova-plugin-googlemaps](https://github.com/setreuid/cordova-plugin-googlemaps)에서 README.md 한글화 하였습니다.

## [HTTP JSON](https://github.com/setreuid/httpjson)

최근 안드로이드 앱 개발중에 서버와 JSON 통신할 일이 생겨서 만든 자바 라이브러리입니다.

HTTP 통신과 JSON 파싱을 한번에 해결하고, Javascript에서 Dictionary 객체의 하위 객체를 접근하는 것처럼 쉽게 사용하고 싶어 만들었습니다.

기본 POST, GET 메서드를 제공하며 메서드 체이닝(Method Chaining) 방식으로 위에서 언급했던 하위 객체 접근을 용이하게 하였습니다.

현재 문제점으로, Byte[] 객체를 서버에 전송할 수 없어서 파라미터를 전달할때 쓰이는 `HashMap<String, String>`객체 대신 새로운 전달 객체 클래스를 구현할 예정입니다.
