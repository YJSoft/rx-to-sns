# To SNS 애드온
Rhymix에서 글을 등록할 때 X(구 트위터)에 자동으로 글을 올리는 애드온입니다. 무료 API의 경우 월 1,500개의 게시글을 전송할 수 있습니다.

## X API 사용 승인 받기
1. 우선 게시글을 올릴 X 계정으로 로그인합니다.
2. [이 링크](https://developer.x.com/en/portal/petition/essential/basic-info)에 접속합니다.
3. 개인적인 목적으로 사용시 하단 Sign up for Free Account 링크를 눌러 무료 계정을 신청합니다.
4. **Describe all of your use cases of Twitter’s data and API:** 아래쪽에 사용 목적을 영어로 **250글자 이상** 간략하게 적습니다.
5. 예시:
```
I'm a personal site owner. I want to upload posts from my site to my X account at the same time. To do this, I'll utilize the X API to upload the title and link of the uploaded post to X. My site will only upload posts that comply with the X Rules and I will endeavor to comply with them. Thank you.
```

## API 정보 수정 및 API 정보 받기
1. https://developer.x.com/en/portal/dashboard 에 접속합니다.
2. 무료 API 사용 신청이 되었다면 기본 프로젝트와 앱이 자동 생성됩니다.
3. Default project 로 시작하는 환경을 클릭합니다.
4. 기본적으로 숫자로 시작하는 앱이 생성되어 있습니다. App details에서 수정 버튼을 눌러 Name을 수정합니다.
5. User authentication settings 하단에 User authentication not set up 이라고 되어 있는 경우 Set up 버튼을 눌러주세요.
6. App permissions은 Read and write, Type of App은 Web App, Automated App or Bot을 선택합니다.
7. App info 하단 Callback URI / Redirect URL이나 Website URL은 웹사이트 주소를 입력합니다.
8. 만약 같은 앱으로 X 로그인도 구현하시려면 Callback URI / Redirect URL에 소셜로그인 모듈의 콜백 주소를 입력하셔도 됩니다.
9. 자동으로 표시되는 OAuth 2.0 Client ID, Client Secret은 무시하셔도 됩니다.

## API 정보 확인
1. Keys and tokens 탭에서 API Key and Secret 옆 Regenerate 버튼을 누릅니다. API Key와 API Key Secret을 메모해주세요.
2. 하단 Access Token and Secret 에서 Generate 버튼을 누릅니다. Access Token과 Access Token Secret을 메모해주세요.
3. 토큰 생성 후 Created with Read and Write permissions 라고 표시되지 않는다면 위 API 정보 수정 단계를 재진행해주세요.(User authentication set up 옆 Edit 버튼 클릭)
4. 애드온 설정 화면에서 메모해둔 값을 입력 후 저장합니다.
5. 만약 메모해둔 값을 잊었다면 Regenerate 버튼을 눌러 재생성 가능합니다.
