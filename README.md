<img src="https://github.com/user-attachments/assets/a8cbdfb9-e1bd-45cc-8f43-ef63bb77439b" width="100"/> <br/>
# 🎯 프로젝트 개요
### "CI/CD 파이프라인 구축이 처음인 개발자를 위한 배포 자동화 지원 서비스"
<div align="center">
  <img src="https://github.com/user-attachments/assets/d3006826-c136-43db-8604-a6074d9be4df"/>
</div>
<br/>

### 📆 프로젝트 정보
삼성 청년 SW 아카데미 12기 자율 프로젝트 A301 <br/>

주제: 오픈소스 개발 <br/>
기간: 2025.04 ~ 2025.05 (6주) <br/>
인원: 6명 (FE 2명, BE 4명) <br/>
<br/>

### ⭐ 프로젝트 기획 배경
CI/CD 파이프라인 구축 경험이 있는 SSAFY 교육생 26명에게 설문조사를 실시한 결과, <br/>
Jenkins 등의 초기 설정과 배포 스크립트 작성에 가장 큰 어려움을 느끼고 있었습니다. <br/>
또한 로그 확인 어려움, EC2에 직접 접속하여 배포하는 과정에서도 어려움이 있다고 응답했습니다. <br/>

**Devpilot**은 프로젝트 개발 환경과 Git 정보를 입력하면 자동으로 배포 스크립트를 작성하고, 빌드 로그를 제공합니다. <br/>
서비스 이용 도중 궁금한 사항이나 에러를 해결할 수 있도록 AI 챗봇 기능을 지원합니다. <br/>
Jenkins GUI와 유사한 UI를 구현함으로써 추후 Jenkins로 CI/CD 파이프라인 재구축 시 어려움을 덜 겪도록 개발했습니다. <br/>
<br/>

### 🖥️ 기술 스택
|분류|사용 기술|
|:---:|:---:|
|**Backend**|Gradle 8.13, Spring Boot 3.4.2, Powershell Script, Jenkins API|
|**Frontend**|Vite 6.3.1, React 18.3.1, TypeScript 5.7.3, Tailwind CSS 3.4.17|
|**AI**|FastAPI 0.115.12 , ipython 9.0.2, huggingface-hub 0.30.2, langchain 0.3.25, pinecore 6.0.2 |
|**외부 서비스**|pinecore - 대규모 벡터 데이터를 효율적으로 검색할 수 있도록 지원하는 클라우드 기반 벡터 DB|
<br/>

# 🚀 주요 기능

### 1. 대시보드
* Devpilot의 메인 화면으로, 프로젝트별 가장 최근에 진행한 빌드 결과를 조회할 수 있습니다.
* 빌드 결과는 아이콘으로 확인 가능하며, 로그를 조회할 수 있는 페이지로 즉시 이동할 수 있습니다.

### 2. 프로젝트 정보 입력
* Dockerfile, Jenkinsfile 생성을 위한 프로젝트 개발 환경과 Git 정보를 입력할 수 있습니다.
* 개발 환경 오기입으로 인한 오류를 방지하고자 입력폼 유효성 검사가 수행됩니다.
* Spring boot 백엔드와 React 프론트엔드 프로젝트에 대하여 구현되었으며, 추후 여러 개발 환경에 대응할 수 있도록 확장할 수 있습니다.

### 3. 빌드 로그 조회
* 빌드 수행 시 실시간으로 로그를 조회할 수 있습니다.
* 빌드가 완료된 프로젝트에 대해서도 로그를 조회하여 에러 발생 지점을 확인할 수 있습니다.
* 대시보드 페이지에서 로그 조회 페이지로 즉시 이동할 수 있습니다.

### 4. AI 챗봇
* 모든 페이지에서 화면 우측 하단의 챗봇 아이콘을 클릭하여 채팅창을 열 수 있습니다.
* Hugging Face 플랫폼의 오픈소스 LLM을 FastAPI로 구현하고, Jenkins 공식 문서 크롤링 후 RAG 기법을 적용했습니다.
* 가장 정확한 답변을 제공한 NVIDIA의 LLaMA 파인튜닝 모델을 챗봇 모델로 선정했습니다.
<br/>

# 📈 성과
* 사용자의 로컬 환경에서 CI/CD 파이프라인을 쉽게 구축할 수 있도록 진입 장벽을 낮췄습니다.
* Electron에서 **Wails**로 Desktop 앱 개발 환경을 전환하여 **앱 용량을 400MB에서 60MB로 줄였**습니다.
* 오픈소스 배포를 목표로 개발하며 **외부 공개 및 확장성**을 고려한 개발 프로세스를 경험했습니다.
<br/>

---
## 👨‍👩‍👧‍👦 팀원 소개
|팀장|FE 리드|FE / Wails 개발|BE 리드|BE|BE / AI 챗봇 구현|
|:---:|:---:|:---:|:---:|:---:|:---:|
|<img src="https://avatars.githubusercontent.com/u/145307456?v=4" width="150"/>|<img src="https://avatars.githubusercontent.com/u/125232426?v=4" width="150"/>|<img src="https://avatars.githubusercontent.com/u/55517023?v=4" width="150"/>|<img src="https://avatars.githubusercontent.com/u/98104967?v=4" width="150"/>|<img src="https://avatars.githubusercontent.com/u/78478247?v=4" width="150"/>|<img src="https://avatars.githubusercontent.com/u/99404991?v=4" width="150"/>|
|[한재서](https://github.com/rpeowiqu)|[유준선](https://github.com/steepheno)|[이지운](https://github.com/isemae)|[김용명](https://github.com/kunzatt)|[이준환](https://github.com/ljh0401)|[박성문](https://github.com/SungMoonPark)|
<br/>

## ⚙️ 아키텍처
<div align="center">
  <img src="https://jsundev.vercel.app/images/devpilot/architecture.png"/>
</div>
<br/>

## 📅 Jira 일정 관리
<div align="center">
  <img src="https://github.com/user-attachments/assets/2945c55c-73bb-44c4-b9c5-3d9bfdfa8918"/>
</div>
