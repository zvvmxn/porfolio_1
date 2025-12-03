Job Platform User Behavior Analysis



(채용 플랫폼 사용자 행동 분석 및 리텐션 인사이트)



📌 프로젝트 개요



채용 플랫폼 서비스에서 사용자 행동 로그 데이터를 기반으로

신규 유저와 가이드 유저 행태 분석,

리텐션(잔존율) 분석,

전환 퍼널 분석,

세분화 및 행동 기반 인사이트 도출을 수행한 프로젝트입니다.



목표는 다음과 같습니다:



사용자 행동 패턴 이해



리텐션 상승 요인 식별



전환 흐름에서의 드롭오프 구간 발견



UX/UI 개선 포인트 도출



실질적인 제품 개선 전략 제시



📁 데이터 구성



사용된 데이터는 플랫폼 로그 및 이력 데이터로 구성됩니다.



주요 테이블 예시:



log\_2022.csv, log\_2023.csv – 행동 로그



log\_URL.csv – URL 기반 액션 정보



job\_platform\_analysis.ipynb – 본 분석 코드 (✔ 현재 repo에 포함)



(+) 모든 raw CSV는 GitHub 업로드 제한으로 제외하고 .gitignore 처리 완료



🔍 주요 분석 내용

1\) URL 기반 사용자 행동 분류



URL 문자열을 기반으로 action type을 생성



예:



회원가입 페이지 진입



회원가입 완료



공고 상세 조회 (view\_job)



회사 정보 조회 (company\_view)



지원 단계(step1~step4) 진행



지원서 제출 완료 (apply\_submit)



이를 통해 정량적 액션 매핑 가능



2\) 사용자 유형 구분



신규 vs 기존 사용자(new\_user)



가이드 유저 vs 일반 유저(guide\_flag)



세그먼트별 행동 및 리텐션 비교



3\) 리텐션 분석 (Retention / Cohort 분석)



주요 결과:



구분	30일 리텐션

전체 유저	53.5%

신규 유저	(lower)

가이드 유저	(higher)



가이드 액션을 수행한 유저는 서비스에 잔존할 확률이 높음

→ Guided onboarding은 retention에 유의미한 기여



4\) 퍼널 분석 (가입 → 조회 → 북마크 → 지원 → 제출)



예시:



단계	가이드 유저	비가이드 유저

view\_job	93.6%	74.7%

company\_view	88.7%	55.9%

bookmark	42.8%	10.9%

apply\_step	61.9%	24.2%

apply\_submit	55.5%	17.3%



→ 가이드 유저는 이후 단계로 넘어갈 확률이 훨씬 높음



🧠 인사이트 요약 (핵심 포인트)

✔ 가이드 기능은 강력한 Engagement Booster



Guided onboarding이 행동 활성화를 유도



정보 탐색 → 관심 확장 → 지원 확률 증가



✔ 신규 유저는 초반 드롭이 크다



첫 5일 retention 개선이 핵심



“초기 경험 설계”가 중요



✔ 북마크(bookmark)는 강력한 전환 지표



북마크 수행자는 지원 확률이 유의미하게 증가



북마크를 유도하는 UI 보강 필요



💡 제품 개선 전략 제안

1\) 신규 유저 온보딩 강화



첫 방문 시 추천 직무/기업 개인화



행동 가이드 표시



2\) 가이드 액션 구조 확대



“다음으로 할 행동 제안”



북마크 추천:

“이 공고도 관심 있어할 것 같아요”



3\) 지원 프로세스 단순화



redundant 입력 제거



지원서 자동완성 기능 강화



4\) 리텐션 지표 개선



7일/30일 잔존율 실시간 대시보드 운영



A/B testing을 통한 UX 개선



🛠 기술 스택



Python (pandas, numpy)



Jupyter Notebook



EDA, 퍼널 분석, 코호트 분석



SQL 기반 데이터 처리



Git / GitHub 버전 관리



📎 파일 안내

파일	설명

job\_platform\_analysis.ipynb	전체 분석 코드 및 시각화

.gitignore	데이터 파일 제외

🙌 프로젝트 의의



이 프로젝트는 단순 EDA를 넘어:



실제 제품 개선 전략



사용자 행동 기반 의사결정



Retention 중심 사고

를 반영하는 작업입니다.



포커스는 “사용자를 남게 만드는 서비스란 무엇인가?”

그리고 “어떤 행동이 잔존과 전환을 만든가?” 입니다.



✉️ 문의 / 연락

구분	정보

GitHub	https://github.com/zvvmxn



Email		jm575496@gmail.com

