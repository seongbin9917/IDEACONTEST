# 개요
2019년도 1학기 캡스톤디자인 프로젝트 관리 페이지입니다.

# 팀
- 팀명 : 0227
- 팀원 및 역할
    - 임병준 : 프로젝트 진행 총괄 & 서류 작성 & 자동화 스크립트 작성 & 오픈소스 활용 가능성 검토 & 기타 프로그램 작성 & professor 구현 & Git 관리
    - 염희수 : 데이터베이스 생성 & 관리, 회의록 작성 & SQL 질의 작성 & 테스트 데이터 간 유효성 검사
    - 이상욱 : 웹페이지 레이아웃 초안 작성
    - 정재민 : 서버 구축 & 관리 & student 구현

# 주제 및 기대효과
  - 프로젝트명 : SCode
  - 학교 실습 시스템을 보다 효율적으로 관리하기 위한 새로운 실습관리 페이지
  
  - 기대효과
    - 모든 과제를 하나의 웹 플랫폼에서 진행이 가능하며, 별도로 플랫폼을 추가 구성할 필요가 없음
    - 과제 이력을 개개인이 github로 업로드할 필요가 없음
    - 각종 통계자료를 교육 개선 등에 활용 가능
  
# 기능  
  - 학생들은 자신의 과제를 압축하여 올리지 않고, 페이지 내에서 코드를 작성 및 제출이 가능
  - 기존의 실습환경과 달리 교수(조교)의 채점이 아닌 testcase를 통한 자동 채점이 가능
  - 학생들 개개인의 실습결과물이 자신의 github에 일괄 등록되어 github를 효율적으로 관리
  - 문제별 정답률, 풀이시간, 성능 등의 자료를 수집하여 통계자료를 제공
    
# 회의록 
- [2019.03.13(수)](https://github.com/BJ-Lim/Capstone_Design/tree/master/minutes/1.md)
- [2019.03.16(토)](https://github.com/BJ-Lim/Capstone_Design/tree/master/minutes/2.md)
- [2019.03.23(토)](https://github.com/BJ-Lim/Capstone_Design/tree/master/minutes/3.md)
- [2019.03.29(금)](https://github.com/BJ-Lim/Capstone_Design/tree/master/minutes/4.md)
- [2019.04.24(수)](https://github.com/BJ-Lim/Capstone_Design/tree/master/minutes/5.md)
- [2019.04.29(월)](https://github.com/BJ-Lim/Capstone_Design/tree/master/minutes/6.md)

# 디렉토리 구조
```
OSS_analysis        오픈소스 활용 가능성 검토 관련 디렉토리
auto_script         서버 환경 구성을 위한 자동화 스크립트 관련 디렉토리
capture_ref         대부분의 캡쳐 이미지가 위치
database            데이터베이스 관련 디렉토리
docs                프로젝트 문서 관련 디렉토리
minutes             회의록
samples             서버의 기능을 테스트하기 위한 예제 파일들이 위치한 디렉토리
server              서버환경 구성 테스트 관련 디렉토리
src                 기타 필요한 연결 프로그램 소스코드 및 Django 코드
trouble_shooting    프로젝트를 진행하며 발생한 문제사항들 정리
```

# Documentation
- 이 문서는 [Document](https://github.com/BJ-Lim/Capstone_Design/tree/master/docs)와 동일한 내용입니다.

## 사전 지식
- 이 아이디어에 대하여 보다 쉽게 이해를 하기 위해서는 다음과 같은 사전지식이 있으면 도움이 될 것입니다.
  - 기존의 비슷한 아이디어의 문제점
  - 오픈소스 SW에 관한 지식
  - 아이디어가 어플로서 구현되기 위한 다양한 조건(ex- 구현순서, 구현 방법 등) 
  - 기존에 존재하는 주차공간 확인 시스템에 이용되는 다양한 센서의 종류
  - 센서들의 작동원리 구현 방법에 대한 것

## 핵심 문서
문서명 | 설명
---- | ----
[URL 패턴](https://github.com/BJ-Lim/Capstone_Design/blob/master/docs/URL_pattern.md) | 웹 페이지의 URL을 정의해 놓은 문서
[Django 폴더 구조](https://github.com/BJ-Lim/Capstone_Design/blob/master/docs/directory_structure.md) | 이 프로젝트에 사용된 Django의 디렉토리 구조
[judgeManager.py](https://github.com/BJ-Lim/Capstone_Design/blob/master/docs/judgeManager.md) | 이 프로젝트와 오픈소스 프로젝트인 [dmoj-judge](https://github.com/DMOJ/judge)를 연결하기 위한 클래스
[page_parameters](https://github.com/BJ-Lim/Capstone_Design/blob/master/docs/page_parameters.md) | 각각의 페이지에서 다른 페이지로 넘어갈 때 넘겨주는 파라미터들을 정의해 놓은 문서
[데이터베이스(스키마)](https://github.com/BJ-Lim/Capstone_Design/blob/master/database/database.md) | 스키마 구조를 정의해 놓은 문서
[데이터베이스(SQL)](https://github.com/BJ-Lim/Capstone_Design/tree/master/database) | SQL을 정의해 놓은 문서
[데이터베이스(E-R 다이어그램)](https://github.com/BJ-Lim/Capstone_Design/blob/master/database/ERD_0227_v3.PNG) | E-R 다이어그램을 정의해 놓은 문서(최신화 되어있지 않음)
[테스트 상황](https://github.com/BJ-Lim/Capstone_Design/blob/master/docs/test.md) | 이 프로젝트에서 테스트 하기 위한 상황을 가정하고 설명한 파일

## 참고 문서
문서명 | 설명
---- | ----
[오픈소스 활용 가능성 검토](https://github.com/BJ-Lim/Capstone_Design/tree/master/OSS_analysis) | 이 프로젝트를 위한 여러 오픈소스 비교 및 활용 가능성 검토
[MariaDB 기본 명령어](https://github.com/BJ-Lim/Capstone_Design/blob/master/database/db_command.md) | 마리아 DB의 기본 명령어 및 설치법

## 개선 해야할 점
- 해당 아이디어를 어플로 구현하고 실행을 하는데 오류를 줄여나가기 위한 구체적 방안을 구상.
  - 현재 존재하는 어플의 기능에서 나아가 구체적인 기능들을 추가한 만큼 추가한 부분으로 인해 오류가 생기지 않도록 적절한 방안을 구상하면 사용자가 사용하는데 있어서 편의성 뿐만 아니라 안정성도 보다 강화 될 것 입니다.
- 해당 아이디어를 구현하는데 있어서 현존하는 다른 다양한 오픈소스SW에 대한 조사.
  - 단순히 어느 한 오픈소스SW를 이용하기 보다는 이에 적합한 다양한 것들에 대하여 조사하고 적용함으로써 보다 심도있고 구체저긴 구현이 가능 할 것입니다.
- 언어 설정
  - 현재 아이디어에서는 언어를 설정할 수 있는 방법이 없습니다. 언어 설정이 가능한 기능을 구현한다면 어플을 사용하는 사용자 폭이 더 넓어질 것입니다.
- 물품위치 정보 시스템을 구현하기 위한 도구
  - 물품위치 정보 시스템을 구현하기 위해서 wi-fi 나 비콘 등에 대하여 생각을 해보았는데 이밖에도 오류의 빈도가 더 적고 구현이 쉬운 것을 구현하면 보다 완성도가 높은 시스템이 될 것 입니다.
- 디자인
  - 현재는 어플의 대략적인 디자인 요소들에 대해서만 간단히 구현을 하였는데 차후에 완성된 어플에는 디자인 요소들에게 있어서도 작은 부분까지 디테일을 살려 완성도를 높일 것 입니다. 
- 보안기능
  - 현재는 아이디어에 대해서만 간략히 설명 하였기 때문에 어플의 보안에 대해서는 구체적인 구현 방식에 대하여 생각해보지 않았지만 이 또한 차후에 완성 어플에서는 구체적으로 구현함으로써 어플의 보안 안정성을 높일 것 입니다.
