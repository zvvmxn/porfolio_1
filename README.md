Job Platform User Behavior Analysis

채용 플랫폼 사용자 행동 분석 및 리텐션 인사이트

📌 프로젝트 개요

채용 플랫폼 서비스에서 사용자 행동 로그 데이터를 기반으로
신규 유저와 가이드 유저 행태 분석,
리텐션(잔존율) 분석,
전환 퍼널 분석,
세분화 및 행동 기반 인사이트 도출을 수행한 프로젝트입니다.

📁 데이터 구성

job_platform_analysis.ipynb – 전체 분석 코드

행동 로그 CSV 파일 (GitHub 용량 제한으로 제외 / .gitignore 처리)

🔍 주요 분석 내용
1) URL 기반 액션 분류

회원가입 페이지 진입

회원가입 완료

공고 상세 조회 (view_job)

회사 정보 조회 (company_view)

지원 단계 (apply_step)

지원서 제출 완료 (apply_submit)

2) 사용자 유형 구분

신규 유저 vs 기존 유저

가이드 유저 vs 일반 유저

3) 리텐션 분석
구분	30일 리텐션
전체 유저	약 53.5%
신규 유저	낮음
가이드 유저	높음
4) 퍼널 분석

가이드 유저가 모든 단계에서 더 높은 전환율을 보임.

🧠 핵심 인사이트

✔ 가이드 기능은 Engagement를 크게 높임
✔ 신규 유저의 초기 이탈이 크므로 온보딩 중요
✔ 북마크(bookmark)는 지원 가능성을 높이는 핵심 지표

💡 제품 개선 전략

신규 온보딩 강화

가이드 액션 구조 확장

지원 프로세스 단순화

리텐션 지표 모니터링

🛠 기술 스택

Python, pandas, numpy

Jupyter Notebook

SQL

Git / GitHub

✉️ Contact

GitHub: https://github.com/zvvmxn