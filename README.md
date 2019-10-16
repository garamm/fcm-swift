# fcm-swift Firebase 연동 순서

1. 프로젝트 생성  
  
2. https://firebase.google.com 접속  
  
3. 시작하기 클릭  
![readme-1](./img/readme-1.png)
  
4. 프로젝트 추가  
![readme-2](./img/readme-2.png)
  
5. iOS 선택  
![readme-3](./img/readme-3.png)
  
6. Firebase에서 제시하는 대로 진행  
참고) Podfile 입력 시  
pod 'Firebase/Messaging'  
이것도 추가로 입력해야 함  
  
7. https://developer.apple.com/account/resources/ 접속  
  
8. Key 추가  
![readme-4](./img/readme-4.png)
  
9. Apple Push Notifications service (APNs) 체크 후 Continue 버튼 클릭  
![readme-5](./img/readme-5.png)
  
10. Register 버튼 클릭  
![readme-6](./img/readme-6.png)
  
11. AuthKey_blabla.p8 파일 다운로드 받은 후 Done 버튼 클릭(파일 보관하고 있기, Key ID 기억해두기)  
![readme-7](./img/readme-7.png)
  
12. Identifiers 추가  
![readme-8](./img/readme-8.png)
  
13. App IDs 선택 후 Continue 버튼 클릭  
![readme-9](./img/readme-9.png)
  
14. Bundle ID 입력하고 스크롤해서 Push Notifications에 체크 후 Continue 버튼 클릭 후 Register 버튼 클릭  
![readme-10](./img/readme-10.png)
![readme-11](./img/readme-11.png)
  
15. Firebase 콘솔로 돌아가서 iOS 설정 버튼 클릭  
![readme-12](./img/readme-12.png)
  
16. 설정 > 클라우드 메시징 > iOS 앱 구성 에서 APN 인증키 업로드 버튼 클릭  
![readme-13](./img/readme-13.png)
  
17.  인증키, 키 ID, 팀 ID 입력  
인증키 : 11번에서 다운로드 받았던 .p8 파일 업로드  
키 ID : 11번에서 기억해두었던 키값  
팀 ID : ? 버튼 클릭 후 조회 가능  
![readme-14](./img/readme-14.png)
  
18. Xcode로 돌아와서 프로젝트 > Signing & Capabilities > + Capability > Notification 선택  
![readme-15](./img/readme-15.png)
  
19. 코드 작성  
