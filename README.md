# 🏦 5조 / HRBANK 인적 자원 관리 시스템
<div align ="center">
  
  ![macbook](https://github.com/user-attachments/assets/06a5e48e-f3cf-4d2a-ba6d-f706aef9d5fb)
  
**HRBANK [🔗 지금 이용해보러가기](https://sb01-hrbank-team05-production.up.railway.app/)**
</div>


## 프로젝트 소개
- **HRBANK**는 기업의 인적 자원을 안전하게 관리하는 서비스입니다.
- Batch로 데이터를 관리하는 Open EMS입니다.
- 직원, 부서들을 추가 혹은 수정이 가능합니다.
- 수정이력이 실시간으로 남고 백업 요청 시 csv로 파일 다운로드 받을 수 있습니다.

## 개발 기간
- 데이터 베이스 설계, 규칙 설계 : 2025.03.13 ~ 2025.03.14 (2days)
- 기능 구현 : 2025.03.14 ~ 2025.03.22 (9days)
- 리팩토링 : 2025.03.24 ~

## 작업 방식
- 오전 스크럼 1회 (09:00 ~ 09:30)
- 예상치 못한 버그 발생은 깃 이슈 작성

## 함께한 팀원
<div align= "center">
  
  |강소율|이소영|이규셕|전성삼|오하람|
  |:---:|:---:|:---:|:---:|:---:|
  |<img width="160" alt="image" src="https://github.com/user-attachments/assets/b0c2314f-8c9e-4dab-8caa-a6b4c29bce44">|<img width="160" alt="image" src="https://github.com/user-attachments/assets/57d56c9d-7438-4e89-90de-5b219c45e132">|<img width="160" alt="image" src="https://github.com/user-attachments/assets/8f7f6fbb-b867-4afe-94be-d478dc556547">|<img width="160" alt="image" src="https://github.com/user-attachments/assets/92567bfc-2186-4e1e-849d-b92b843bff70">|<img width="160" alt="image" src="https://github.com/user-attachments/assets/0f51714c-e0b6-4b0c-a755-acb7230915d7">|
  |[@soyul9280](https://github.com/soyul9280)|[@gitSoyoungLee](https://github.com/gitSoyoungLee)|[@impmonzz](https://github.com/impmonzz)|[@hodu31](https://github.com/hodu31)|[@Haram0111](https://github.com/Haram0111)|

</div>

## 프로젝트 목표
- 그동안 배운 기술 스택으로 서비스 만들어보기
- PR, 깃이슈 열심히 작성하기
- 완결보다 완성하기

## 기술스택
<div align= "center">
  <span>
  <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white">
  <img src="https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white">
  <img src="https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white">
  <img src="https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white">
  <img src="https://img.shields.io/badge/springjpa-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white">
  <img src="https://img.shields.io/badge/railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white">
  </span>
</div>

<br>
<br>


## 역할 분담
### 강소율 (Leader)
- 직원 수 추이 API
- 총 직원수 API
- 부서별 / 직함별 직원 분포 API
- 파일 다운로드 API
  
### 이소영
- 직원 정보 수정 이력 목록 조회 API
- 직원 정보 수정 이력 상세 조회 API
- 수정 이력 건수 조회 API

### 전성삼
- 파일 다운로드 API
- 직원 등록 API
- 직원 목록 조회 API
- 직원 상세 조회 API
- 직원 삭제 API
- 직원 수정 API

### 이규석
- 부서 목록 조회 API
- 부서 등록 API
- 부서 상세 조회 API
- 부서 삭제 API
- 부서 수정 API

### 오하람
- 데이터 백업 목록 조회 API
- 데이터 백업 생성 API
- 최근 백업 정보 조회 API
  
## 폴더구조

```
📦src
 ┣ 📂main
 ┃ ┣ 📂java
 ┃ ┃ ┣ 📂com
 ┃ ┃ ┃ ┣ 📂codeit
 ┃ ┃ ┃ ┃ ┣ 📂demo
 ┃ ┃ ┃ ┃ ┃ ┣ 📂config
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜QueryDslConfig.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜SwaggerConfig.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜WebConfig.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂controller
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂api
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentApi.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogApi.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentApi.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeApi.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupController.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentController.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogController.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentController.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeController.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂dto
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂data
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜CursorPageResponseChangeLogDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜CursorPageResponseDepartmentDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜CursorPageResponseEmployeeDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DiffDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeDistributionDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeTrendDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂request
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentCreateRequest.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentUpdateRequest.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeCreateRequest.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeUpdateRequest.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📂response
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupHistoryDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜CursorPageResponseBackupDto.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜ErrorResponse.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂entity
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂enums
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupStatus.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeType.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmploymentStatus.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜PropertyName.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜Backup.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContent.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescription.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLog.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜Department.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜Employee.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂exception
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentNotFoundException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DuplicateEmailException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeNotFoundException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜FileNotFoundException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜FileStorageException.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜GlobalExceptionHandler.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂mapper
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescriptionMapper.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogMapper.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentMapper.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeMapper.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂repository
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescriptionRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogCustomRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogCustomRepositoryImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentRepositoryCustom.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentRepositoryImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeRepository.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeStatsRepository.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂service
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📂impl
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescriptionImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeServiceImpl.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BackupService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeDescriptionService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ChangeLogService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜DepartmentService.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜EmployeeService.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂storage
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentStorage.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜LocalBinaryContentStorage.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📂util
 ┃ ┃ ┃ ┃ ┃ ┃ ┣ 📜ClientInfo.java
 ┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜CursorPageUtil.java
 ┃ ┃ ┃ ┃ ┃ ┗ 📜HrbankApplication.java
 ┃ ┃ ┃ ┃ ┗ 📜.DS_Store
 ┃ ┃ ┃ ┗ 📜.DS_Store
 ┃ ┃ ┗ 📜.DS_Store
 ┃ ┣ 📂resources
 ┃ ┃ ┗ 📂static
 ┃ ┃ ┃ ┣ 📂assets
 ┃ ┃ ┃ ┃ ┣ 📂images
 ┃ ┃ ┃ ┃ ┃ ┗ 📜default-profile.svg
 ┃ ┃ ┃ ┃ ┗ 📜index-CKRSZsvY.js
 ┃ ┃ ┃ ┣ 📜favicon.ico
 ┃ ┃ ┃ ┗ 📜index.html
 ┃ ┗ 📜.DS_Store
 ┣ 📂test
 ┃ ┣ 📂java
 ┃ ┃ ┗ 📂com
 ┃ ┃ ┃ ┗ 📂codeit
 ┃ ┃ ┃ ┃ ┗ 📂demo
 ┃ ┃ ┃ ┃ ┃ ┣ 📜BinaryContentServiceTest.java
 ┃ ┃ ┃ ┃ ┃ ┣ 📜EmployeeTest.java
 ┃ ┃ ┃ ┃ ┃ ┗ 📜HrbankApplicationTests.java
 ┃ ┗ 📂resources
 ┃ ┃ ┗ 📂static
 ┃ ┃ ┃ ┣ 📂assets
 ┃ ┃ ┃ ┃ ┣ 📜index-CpuUHdy1.js
 ┃ ┃ ┃ ┃ ┗ 📜index-kQJbKSsj.css
 ┃ ┃ ┃ ┣ 📜favicon.ico
 ┃ ┃ ┃ ┗ 📜index.html
 ┗ 📜.DS_Store
```

## 주요 기능
- 대시보드
  - 직원 정보, 수정 이력, 데이터 백업 관련 정보 조회
  - 직원 증감 그래프 조회
 
- 부서관리
  - 부서 등록, 수정, 삭제, 검색
 
- 직원관리
  - 직원 등록, 정보 수정, 삭제, 상세 조회, 검색
 
- 수정이력
  - 직원 정보 수정 이력 관리 및 검색
 
- 데이터백업
  - 새 백업 생성 (요청 및 배치 백업 지원)
  - 파일 다운로드
  - 조회 검색

## 목차
- [메인페이지](#main-page)
- [직원 페이지](#employee-page)
- [백업 페이지](#backup-page)


## 📃 페이지 구성
## <a id="main-page"></a>1. 메인페이지
![main](https://github.com/user-attachments/assets/fdbf6635-1ba6-44c6-b48d-a784e7a49011)

- 서비스를 접속하면 가장 처음 나타나는 화면입니다.
- 총 4개의 섹션으로 구분되어있습니다.
  - 메뉴
  - 총 직원수, 수정이력 등 정보 조회
  - 주어진 시간 조건에 따른 직원 수 추이
  - 부서별/직함별 직원 수 조회 
  
### 메인페이지에서 사용한 기능
- `QueryDsl`을 이용한 조건별 조회
- `IntStream.iterate` 를 사용하여 주어진 시간 조건 별 기간 생성
- 시간 조건 별로 직원 수 증감 변화 조회

### 앞으로 개발할 기능
- [직원 수 증감]
  주어진 시간 조건 별 기간 List로 반복문을 돌며 count쿼리가 시행되어 그래프 로드가 느립니다. 반복문 밖으로 빼내어 로드가 빨리되도록 해야합니다.

## <a id="employee-page"></a>2. 직원 페이지
![직원 ](https://github.com/user-attachments/assets/149c6e78-5e68-4b17-9cb8-1d2248d212c1)

- 프로필 이미지를 등록할 수 있습니다.
  
### 회원가입 페이지에서 사용한 기능
- byte는 로컬 폴더에 저장하도록 설정하였습니다.

## <a id="backup-page"></a>3. 백업 페이지
![백업](https://github.com/user-attachments/assets/de5be6b2-3241-4c9b-b77b-5fcda6e5a602)

- 직원정보를 수정한 뒤 백업 요청을 시행하면 파일을 다운로드 받을 수 있습니다.
- 1시간동안 직원정보 수정이 안되었을 때 백업 요청을 하면 건너뜀 상태로 생성됩니다.
  
### 백업 페이지에서 사용한 기능
- UTF8-BOM을 사용하여 csv파일 다운로드 시 한글깨짐을 방지하였습니다.

### 앞으로 개발할 기능
- 1시간마다 백업 파일이 생성되도록 진행해야합니다.


**협업 문서 [🔗 notion](https://agate-spectacles-6eb.notion.site/1b5c5631fb0180f6aee4ccdd7b897b74?pvs=4)**

**회고 문서 [🔗 notion](https://valley-anglerfish-fc3.notion.site/ebd/1bff065c355f8046a25ff633c6382316)**
