LeetCode 코딩 문제들에 대해, 생성 모델들의 소스 생성 능력 검증을 위한 소스코드 저장소입니다.
- LeetCode 사이트: https://leetcode.com/

- Environment
  - 한글 주석 인코딩
    - python 3.X 버전 사용
    - 2.X버전은 # -*- coding: utf-8 -*- 구문 추가해야 함
  - pandas 설치
  - openai 설치

- LeetCode CLi
  - 참고: https://github.com/skygragon/leetcode-cli
  - node.js 설치 필요
  - cmd에서 leetcode user -c 명령어로 로그인후 사용


## 상세설명
### 목표: chat GPT가 잘 생성하지 못하는 코드 발견하기


### get_template.py
-leetcode cli 사용

-leetcode_dataset.csv에 python template과 c template 추가


### leetcodedb.ipynb
-chat GPT에게 leetcode 문제를 3가지 방법으로 질문
1. first result: code template + description 
2. second result: code template + description + constraints
3. third result:  code template + description + constraints + example


### leetcode_submit.py
-leetcode cli 사용

-chat GPT가 생성한 코드를 파일로 저장 후 leetcode에 submit

-submit 결과를 통해 chat GPT가 잘 생성하지 못하는 코드 발견 가능


### registration_date.ipynb
-http://web.archive.org/ 참고

-leetcode 문제가 등록된 날짜 확인

-leetcode가 이미 chat GPT 학습에 활용되었을 가능성 때문


### leetcode cli 사용법
-https://github.com/skygragon/leetcode-cli

-node.js 설치

-로그인 방법: leetcode user -c
