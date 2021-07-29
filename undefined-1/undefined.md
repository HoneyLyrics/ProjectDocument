# 로그인 및 회원가입 명세



```text
 회원가입
    - Method: POST
    - URL: /api/auth/register
    - 요청: (이메일), 아이디, 비밀번호

      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |username|String|Y|아이디 겸 유저명|
      |password|String|Y|비밀번호|

    - 응답
      
      StatusCode: 200
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |username|String|Y|아이디, 유저 확인용|
      
      StatusCode: 400(Bad Request)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |error|String|Y|실패원인|

      StatusCode: 409(Conflict)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |error|String|Y|실패원인|
      
      StatusCode: 500(Internel Server error)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |error|String|Y|실패원인|      

  - 로그인
    - Method: POST
    - URL: /api/auth/login
    - 요청: (이메일), 아이디, 비밀번호

      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |username|String|Y|아이디 겸 유저명|
      |password|String|Y|비밀번호|

    - 응답
      
      StatusCode: 200
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |username|String|Y|아이디, 유저 확인용|
      
      StatusCode: 401(Unauthorized)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |username|String|Y|아이디, 유저 확인용|
      |error|String|Y|실패원인|
      
      StatusCode: 500(Internel Server error)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |error|String|Y|실패원인|

  - 로그아웃
    - Method: POST || GET
    - URL: /api/auth/logout
    - 응답
      
      StatusCode: 204(No Content)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |username|String|Y|아이디, 유저 확인용|
      
      StatusCode: 500(Internel Server error)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |error|String|Y|실패원인|
      
  - 회원 확인
    - Method: GET
    - URL: /api/auth/check
    - 응답
      
      StatusCode: 200
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |username|String|Y|아이디, 유저 확인용|
      
      StatusCode: 401(Unauthorized)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |error|String|Y|실패원인|
      
      StatusCode: 500(Internel Server error)
      |요청변수|타입|필수 여부|설명|
      |-------|---|---|---|
      |error|String|Y|실패원인|
```

