# RestAPI 명세

### 1. 음악 검색 RestAPI

{% api-method method="get" host="https://honeylyrics.herokuapp.com" path="/musiclist/mooidid=:id" %}
{% api-method-summary %}
get musiclist
{% endapi-method-summary %}

{% api-method-description %}
24가지 감정을 id로 매핑한 값 요청 
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="mooidid" type="string" required=false %}
24가지 감정을 id로 매핑한 값 
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
music 음악 id, 가수, 제목, 이미지 주소, 가사들을을 담은 json 리스트 
{% endapi-method-response-example-description %}

```
[{"songId": 8130796, "singer": "라붐 (LABOUM)", "title": "상상더하기", "imgURL": "https://cdnimg.melon.co.kr/cm/album/images/026/77/681/2677681_500.jpg?2a966dccb6f2d4c31b4fc5446f315e5d/melon/resize/282/quality/80/optimize", "lyrics": "1 2 Come On R U Ready\n3 4 Do It I'm Ready \n5 6 Baby Are You Ready\n지금 나와 어디든 가자 \n지루한 하루 여기까지만 All Stop\n작은 가방 운동화 챙겨 \n자 더 크게 Radio를 높이고\n코발트블루 물결 눈부신 바다\n달빛 가득 묻은 작은 섬\n야경이 눈부신 도시는 어때\n함께라면 어디든 좋아 난\n너와 나 그곳으로 떠나는 거야 \n상상에 상상에 상상을 더해서\n어머 깜짝야\n눈부셔 눈부셔 눈부셔 이건 뭐\nOh Hello New World \n두 손 모아 소리치면\n푸른 하늘이 내게로 와\n날아가볼래\n상상의 상상의 미래로 가볼까\n바람을 타고 \n새로운 눈빛에 가슴이 붐 붐 붐\nOh 발견했어 우리들만의 Paradise\n흑백영화 같은 하루에 \n레몬 터지듯 짜릿함이 필요해\n지금 당장 널 데려갈게 \n꿈꿔오던 사진 속 그곳으로\n민트그린빛 바람 가득한 숲 속\n달콤한 향기의 칵테일\n지도를 벗어나 Ticket To The Dream\n함께라면 어디든 좋아 난 \n너와 나 그곳으로 떠나는 거야 \n상상에 상상에 상상을 더해서\n어머 깜짝야 \n눈부셔 눈부셔 눈부셔 이건 뭐\nOh Hello New World \n두 손 모아 소리치면\n푸른 하늘이 내게로 와\n날아가볼래\n상상의 상상의 미래로 가볼까\n바람을 타고 \n새로운 눈빛에 가슴이 붐 붐 붐 \nOh 발견했어 우리들만의 Paradise\n너와 나의 비밀스런 풍경들\n언제라도 다시 와 주겠니\n은하수 아래 밤새 부른 노래 \n영원히 잊지 않을 거야\n이 시간 속에 영원히 \n네 품에 안기고 싶은걸 \n단 둘이 이순간 잠들고 싶은걸\n지도엔 없는 이 곳을 꼭 기억해줘\n우리들만의 Paradise \n상상에 상상에 상상을 더해서\n어머 깜짝야\n눈부셔 눈부셔 눈부셔 이건 뭐\noh Hello New World \n처음 만난 세상 속에\n나의 가슴이 라 라 라 라\n날아가볼래\n상상의 상상의 미래로 가볼까\n바람을 타고 \n새로운 눈빛에 가슴이 붐 붐 붐\nOh 발견했어 우리 들만의 Paradise\n1 2 Come On R U Ready\n3 4 Do It I'm Ready \n5 6 Baby Are You Ready"}]
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=500 %}
{% api-method-response-example-description %}
 internal server
{% endapi-method-response-example-description %}

```
{'error':'error message'}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://honeylyrics.herokuapp.com" path="/song/songid=:id" %}
{% api-method-summary %}
 song
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

### 2. 로그인 Rest API

{% api-method method="post" host="https://honeylyrics.herokuapp.com/api/auth/Login" path="/api/auth/Login" %}
{% api-method-summary %}
Login API
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-form-data-parameters %}
{% api-method-parameter name="password" type="string" required=false %}
user password
{% endapi-method-parameter %}

{% api-method-parameter name="username" type="string" required=false %}
userid
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://honeylyrics.herokuapp.com/api/auth/check" path="/api/auth/check" %}
{% api-method-summary %}
Session Check API
{% endapi-method-summary %}

{% api-method-description %}
check if login session is lasting 로그인 세션이 유지되고 있는지 확인합니다.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Cookie" type="string" required=false %}
Cookie 로그인 세션
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="password" type="string" required=true %}
user password
{% endapi-method-parameter %}

{% api-method-parameter name="username" type="string" required=true %}
user id
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
username: username
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{'error':'unauthoized'}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=500 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{'error':errormsg'}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

