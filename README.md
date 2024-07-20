### `comment README.md`

#### `judy-community-backend-comment`

# Judy Community Comment Backend

댓글 관리 및 관련 작업을 처리하는 백엔드 서비스입니다.

## 구조

```
judy-community-backend-comment/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── judycorp/
│   │   │           └── comment/
│   │   │               ├── config/
│   │   │               ├── controller/
│   │   │               ├── dto/
│   │   │               ├── entity/
│   │   │               ├── exception/
│   │   │               ├── repository/
│   │   │               ├── service/
│   │   │               └── ApplicationComment.java
│   ├── resources/
│   │   └── application.properties
├── Dockerfile
├── build.gradle.kts
└── settings.gradle.kts
└── .github/
    └── workflows/
        └── ci-cd.yml
```

## 기능

- 댓글 생성
- 댓글 조회
- 댓글 수정 및 삭제

## 설치 및 실행

### 사전 요구 사항

- [Docker](https://www.docker.com/get-started)
- [JDK 17](https://adoptopenjdk.net/)

### Docker 이미지 빌드 및 실행

```bash
./gradlew build
docker build -t your_dockerhub_username/judy-community-backend-comment .
docker run -p 8084:8080 your_dockerhub_username/judy-community-backend-comment
```

---

### 공통 인프라 `README.md`

# Judy Community Infrastructure

모든 서비스 및 애플리케이션을 관리하는 Docker Compose 설정이 포함되어 있습니다.

## 구조

```
judy-community-infrastructure/
├── docker-compose.yml
├── .env
└── README.md
```

## 기능

- MySQL 데이터베이스 설정
- 각 서비스 및 애플리케이션의 Docker Compose 설정

## 설치 및 실행

### 사전 요구 사항

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Docker Compose 설정 시작

```bash
docker-compose up -d
```
