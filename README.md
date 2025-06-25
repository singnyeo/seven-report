# seven-report
# 초급 프로젝트 SEVEN: 강시연 개발 리포트

## 📌 프로젝트 개요  
**진행 기간**: 2025.06.02 ~ 2025.06.20  
**주제**: 운동 인증 커뮤니티 서비스  
> 사용자가 그룹을 생성하고 원하는 그룹에 참여하여 운동 기록을 남길 수 있는 커뮤니티형 서비스  

**목표**: 프론트엔드 코드와 연동되는 백엔드 API 설계 및 구현

## 💻 기술 스택

| **분류** | **사용 도구** |
| --- | --- |
| Backend | Node.js 22.0.0 LTS (Express) |
| Database | Prisma, PostgreSQL |
| API 문서화 | Swagger |
| 협업 도구 | Discord, GitHub ([🔗 레포지토리](https://github.com/singnyeo/nb02-seven-team2)), Notion ([📃 세부 계획](https://www.notion.so/206fca01d5c980689666cc5d59fbef08?pvs=21)) |
| 일정 관리 | GitHub Issues, Notion |


## 📌 담당 작업

- 기록 랭킹 조회 API 및 기록 상세 조회 API 설계 및 구현
- Prisma ORM 기반 운동 기록 관련 데이터 모델 및 쿼리 최적화
- 페이징 처리, 정렬 조건, 응답 데이터 구조 설계
- GitHub 프로젝트 관리 담당
  - 초기 폴더/파일 구조 설정
  - 브랜치 전략, PR 관리, 커밋 컨벤션 적용
  - README.md 작성


## 🚀 기능 구현

- 기록 랭킹 조회 API
  - 운동 기록 **횟수 기준**으로 주간/월간 랭킹 조회
  - 조회 항목: `닉네임`, `기록 횟수`, `누적 운동 시간`
  - 페이지네이션

- 기록 상세 조회 API
  - 특정 기록의 상세 정보 조회
  - 조회 항목: 운동 종류, 설명, 시간, 거리, 사진(여러장), 닉네임

## 🧠 기술적 성과 
- Prisma ORM 최적화
  - include, select, orderBy, where 등 조합으로 N+1 문제 방지
  - 쿼리 성능 개선 및 relation 데이터 효율적 조회

- RESTful한 API 설계
  - /ranks, /records/:recordid 구조로 명확한 리소스 표현
  - 예측 가능한 응답 포맷

- 유연한 페이징 및 필터 구조
  - skip, take 기반 페이지네이션
  - type=weekly/monthly 등 확장 가능한 쿼리 로직

- GitHub 협업 및 문서화 기여
  - 커밋 컨벤션(feat:, fix:, docs: 등) 적용
  - README 주도 작성
  - 기능 명세 테스트
  - 브랜치 전략, PR 리뷰 기반 개발 경험

## 🎤 발표 및 공유

[📊 중간 발표 자료 ](https://www.miricanvas.com/v/14qg1rp)

* 📢 발표 내용 

-  프로젝트 개요
-  프로젝트 진행상황 공유 등


## 🧪 그룹 API 테스트 보고서

- 프론트엔드 요청 스펙에 맞춘 Postman 테스트 수행  
- Swagger 문서 기준으로 API 동작 여부 일치 확인 

- [🔗 테스트 계획서](https://www.notion.so/seven-210a1c7d0d6a80269a25f5476a37c7a3?source=copy_link)  
- [🔗 테스터 보고서](https://www.notion.so/seven-217a1c7d0d6a80388cdbc33daf0f60da?source=copy_link)

## 🧩 문제점 및 해결 과정

- **Git 협업 방식(Git Flow, 브랜치 전략 등) 생소**  
  - 프로젝트 경험 부족으로 중복 작업과 충돌이 자주 발생함  
  → `feature/기능명` 브랜치 전략과 `feat:`, `fix:` 등 커밋 컨벤션을 정해 통일 사용  

- **이슈 관리 및 팀 내 개발 문화 이해 부족**  
  - PR 리뷰, 커밋 컨벤션 등 협업 규칙 미숙으로 소통이 원활하지 않아 일정 지연  
  → PR을 적극 활용해 작업 내용을 명확히 공유하고 코드 리뷰로 협업 역량 향상  

- **데이터 구조와 API 명세에 대한 문서화 부족**  
  - 실수와 오해 발생  
  → Notion과 README 등 공통 문서에 명세 정리해 실수 줄임  

- **기능 구현 중 발생한 이슈에 대한 소통 부족**  
  - 문제 해결 지연  
  → 디스코드 등으로 즉시 공유하고 해결하는 습관 형성  


## 🔁 회고

- 협업은 **혼자 할 때보다 훨씬 많은 소통과 문서화, 정리 능력**이 필요하다는 걸 체감함
- 단순히 작동하는 코드를 넘어서, **"정확하고 읽기 쉬운 코드"를 어떻게 작성할지**에 대해 많이 고민하게 됨
- 실력도 중요하지만, **작업을 이해시키고 함께 맞춰가는 과정이 더 중요**하다는 걸 배움
- 초기 세팅, 커뮤니케이션 도구, 명세 작성에 대한 중요성을 느낌


## 📎 첨부 
- [🔗 팀 레포지토리](https://github.com/singnyeo/nb02-seven-team2)
- [📚 세부 계획](https://www.notion.so/206fca01d5c980689666cc5d59fbef08?pvs=21)
- [📊 중간 발표 자료](https://www.miricanvas.com/v/14qg1rp)
- [🔗 테스트 계획서](https://www.notion.so/seven-210a1c7d0d6a80269a25f5476a37c7a3?source=copy_link)  
- [🔗 테스터 보고서](https://www.notion.so/seven-217a1c7d0d6a80388cdbc33daf0f60da?source=copy_link)
