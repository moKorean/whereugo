# whereugo
비엠더블유 send to car

https://m.clien.net/service/board/cm_car/12103733

description from 멤피스(clien)

맥만 있으면 가능해 보이긴 합니다. 맥이 있으면 당연히 apple ID 는 있으실 거고, xcode는 apple store에서 무료로 받으면 되는 거라.

대략적인 절차는 이렇네요.
1. 카카오 개발자 계정 생성 (https://developers.kakao.com/)
2. 카카오 개발자 계정에서 [앱 만들기] 요청하여 위 앱에 필요한 key 받기 (네이티브 앱 key, REST API key 필요) (앱이름은 마음대로 하셔도 되요)
3. 카카오 개발자 사이트에서 - 앱이름 - 설정 - 일반 에 가셔서 [플랫폼 추가] iOS 선택하시고 번들 ID 를 자신의 번들 ID를 넣어주세요. (보통 자신 도메인을 꺼꾸로 쓰고 앱이름을 씁니다. 전 com.lomohome.whereugo 로 했었는데 대충 com.영어이름.아까만든앱이름영어 로 하시면 됩니다. com.example.appname)
4. xcode 설치
5. xcode Preference > Account에 자신의 apple ID 등록
6. 위 링크에 있는 project 파일 열기
7. Project의 info.plist에서 2번에서 얻은  자신만의 key 값으로 기존 값 변경 (네이티브 앱 key -> KAKAO_APP_KEY 오른쪽의 [네이티브 앱 키] 라는 부분을 바꾸시고, REST API key -> KAKAO_RESTAPI_KEY : [REST API 키] 의 값을 바꾸시면 됩니다.)
8. 프로젝트파일의 General 탭에서 Bundle Identifier 를 3번과정에서 만든 Bundle Identifier 로 변경합니다.
9. 폰을 맥과 연결
10. Project Target을 연결된 폰으로 지정
11. 빌드

이 과정에서 DEVELOPMENT_TEAM을 자신의 애플 계정(personal-team)으로 설정하고, Bundle Identifier를 나만의 고유한 문자열로 변경하는 등의 변경이 필요합니다. 한번 해 보니 실은 이런 것들이 더 어렵(?)게 보이네요. 여기에 자신의 애플 계정에서 만든 앱을 폰에서 신뢰할 수 있게 하는 절차 등이 필요합니다. 

참고 링크
https://www.egovframe.go.kr/wiki/doku.php?id=egovframework:hyb3.5:hrte:runiphone
https://medium.com/@adie0423/자신의-아이폰에-테스트-앱-올리기-54e07e17d3f7

* 애플 개발자 중에 앱스토어에 올려보실 분은 메일주세요 (mokorean@gmail.com)
