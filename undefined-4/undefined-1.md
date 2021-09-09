---
description: 본 프로젝트에 대해서 설명합니다.
---

# 프로젝트 내용

## 1. 프로젝트 소개

* 본 프로젝트는 노래가사를 감정별로 나누어 검색할 수 있도록 하는 프로그램입니다

## 1. 프로젝트 아키텍처



![&#xC6F9; &#xD504;&#xB85C;&#xC81D;&#xD2B8; &#xC544;&#xD0A4;&#xD14D;&#xCC98;](https://lh6.googleusercontent.com/kTOrYJZDI83AVRdhAZ4hzmaNz8jt89WuBPLPFDt9MnO0A1S_a2IQvyyZfnwz8ats6pDkDiXjSU6czfsQYj3jVPqfstVmMbK-YulS3_opol4KFsSda_5qVPSRfPiPSTG1lL3JjKwd=s0)

1. Front End: UI가 사용자와 직접 상호작용만들었습니다.
2. Heroku-Djangp 모듈: FrontEnd로부터 적절한 요청이 들어오면 그에대한 API가 반응해서 응답합니다.
   * LoingAPI는 회원 가입, 로그인, 로그아웃등 세션관리에 필요한 기능입니다 이느 추후 개인추천을 만들기위해 만들어졌습니다.
   * Music Search API는 감정으로 분류되어있는 음악을 검색할때 필요한 기능입니다.
   * Crawling API는 주기적으로 음악을 가지고오는 기능입니다. 이때 Classification API와 상호작용하여 가사를 감정으로 분류하는 기능이 추가됩니다. 

## 2. 프로젝트의 특징 및 기능 

1. 본프로젝트의 특징은 가사를 자동으로 큐레이팅을 해주는 기능을 가지고 있습니다.
2. 
## 3. 기대 효과 

