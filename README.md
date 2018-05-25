# whereugo
bmw send to car

https://m.clien.net/service/board/cm_car/12103733

description
맥만 있으면 가능해 보이긴 합니다. 맥이 있으면 당연히 apple ID 는 있으실 거고, xcode는 apple store에서 무료로 받으면 되는 거라.

대략적인 절차는 이렇네요.
1. 카카오 계정 생성
2. 카카오 계정에서 앱 생성 요청하여 위 앱에 필요한 key 받기(네이티브 앱 key, REST API key 필요)
3. xcode 설치
4. xcode Preference > Account에 자신의 apple ID 등록
5. 위 링크에 있는 project 파일 열기
6. Project의 info.plist에서 2번에서 얻은  자신만의 key 값으로 기존 값 변경(네이티브 앱 key -> KAKAO_APP_KEY, REST API key -> KAKAO_RESTAPI_KEY)
7. 폰을 맥과 연결
8. Project Target을 연결된 폰으로 지정
9. 빌드

이 과정에서 DEVELOPMENT_TEAM을 자신의 애플 계정(personal-team)으로 설정하고, Bundle Identifier를 나만의 고유한 문자열로 변경하는 등의 변경이 필요합니다. 한번 해 보니 실은 이런 것들이 더 어렵(?)게 보이네요. 여기에 자신의 애플 계정에서 만든 앱을 폰에서 신뢰할 수 있게 하는 절차 등이 필요합니다. 

참고 링크
https://www.egovframe.go.kr/wiki/doku.php?id=egovframework:hyb3.5:hrte:runiphone
https://medium.com/@adie0423/자신의-아이폰에-테스트-앱-올리기-54e07e17d3f7
