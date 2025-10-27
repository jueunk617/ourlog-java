# ✈️ OurLog
> 영화, 음악, 책 감상을 기록하고 나의 취향을 아카이빙하는 콘텐츠 다이어리 플랫폼 (2025.07.22 ~ 2025.08.06)

<br>

## 📚 목차
1. [🖼️ 프로젝트 소개](#️-프로젝트-소개)
2. [👥 팀 구성 및 역할](#-팀-구성-및-역할)
3. [🎯 개발 배경](#-개발-배경)
4. [⚙️ 기술 스택](#️-기술-스택)
5. [🧩 ERD](#-erd)
6. [🧾 API](#-api)
7. [🌐 시스템 아키텍처](#-시스템-아키텍처)
8. [💾 주요 기능](#-주요-기능)
9. [🔄 개발 프로세스](#-개발-프로세스)
10. [🧠 트러블슈팅](#-트러블슈팅)
11. [💡 주요 결정 및 배운 점](#-주요-결정-및-배운-점)

<br>

## 🖼️ 프로젝트 소개
[![pyoji.png](https://i.postimg.cc/y8bYQ1V4/pyoji.png)](https://postimg.cc/tsFj7HZ2)
> **감상을 기록하고 나누는 감성 공유 플랫폼, OurLog**

**OurLog**는 영화·음악·책 등 다양한 콘텐츠 감상을  
하나의 플랫폼에서 기록하고 아카이빙할 수 있는 콘텐츠 다이어리 서비스입니다.  

기존 리뷰 서비스가 단순 별점·한줄평 중심이었다면,  
OurLog는 감정 태그·시각화 통계·공감 피드를 통해  
사용자의 감정과 취향을 데이터로 표현하고 공유합니다.  

<br>

## 👥 팀 구성 및 역할

| 팀원 | 이름 | GitHub | 담당 기능 |
|:------:|:----:|:--------:|:-----------|
| <img src="https://avatars.githubusercontent.com/u/125340502?v=4" width="80px" style="border-radius:10px;"> | **김주은** | [@jueunk617](https://github.com/jueunk617) | • 감상일기 등록 / 수정 / 삭제<br>• 콘텐츠 조회 (영화, 음악)<br>• 백엔드 배포 |
| <img src="https://avatars.githubusercontent.com/u/84756980?v=4" width="80px" style="border-radius:10px;"> | **남기은** | [@namgigun](https://github.com/namgigun) | • 감상일기 조회<br>• 댓글 등록 / 조회 / 수정 / 삭제<br>• 콘텐츠 조회 (도서) |
| <img src="https://avatars.githubusercontent.com/u/127588192?v=4" width="80px" style="border-radius:10px;"> | **노희철** | [@Nohheechul](https://github.com/Nohheechul) | • 통계 카드 (감상 수, 평균 별점, 주요 감정)<br>• 최근 6개월 감상 그래프 / 콘텐츠 분포<br>• 타입·장르·감정·OTT별 그래프 |
| <img src="https://avatars.githubusercontent.com/u/68084426?v=4" width="80px" style="border-radius:10px;"> | **박영빈** | [@yeongbin1999](https://github.com/yeongbin1999) | • 회원가입 / 로그인 / 로그아웃<br>• 내 프로필 조회<br>• 프론트엔드 배포 |
| <img src="https://avatars.githubusercontent.com/u/145415884?v=4" width="80px" style="border-radius:10px;"> | **임종현** | [@dlawhd](https://github.com/dlawhd) | • 타임라인<br>• 팔로우 / 언팔로우<br>• 다른 유저 프로필 조회<br>• 좋아요 기능 |

> 담당 도메인의 프론트엔드 개발 또한 각각 진행함.

<br>

## 🎯 개발 배경

### 🤔 Problem
**“콘텐츠는 많은데, 기록은 부족하다”**

- OTT · 책 · 음악 등 감상 기록이 플랫폼마다 흩어져 있음  
- 기존 리뷰 서비스는 별점 위주로 감정이나 맥락을 담기 어려움  
- 소셜 미디어에 감상을 공개하기에는 부담감이 큼  

<br>

### 💡 해결책
- 🎬 **콘텐츠 유형 통합 관리** (영화, 책, 음악)  
- 💭 **감정 중심의 태그 시스템**으로 세밀한 감정 표현 가능  
- 🔒 **공개/비공개 설정**으로 개인의 프라이버시 보호  
- 📊 **통계·분석 기능**으로 감정 패턴과 취향 시각화  
- 🤝 **팔로우 기반 피드**로 공감과 콘텐츠 발견 제공  

<br>

### ✨ 핵심 가치
📘 **기록** → 📊 **분석** → 🤝 **공유**

OurLog는 단순히 ‘감상’을 남기는 서비스가 아니라,  
감정의 흐름을 데이터로 남기고, 시각화하며,  
타인과 **감정적 연결을 만들어가는 플랫폼**입니다.

<br>

## ⚙️ 기술 스택

### Frontend
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"/> <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=Next.js&logoColor=white"/>

### Backend
<img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=OpenJDK&logoColor=white"/> <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=SpringBoot&logoColor=white"/>

### Database
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/>

### Deployment & Infra
<img src="https://img.shields.io/badge/AWS EC2-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white"/> <img src="https://img.shields.io/badge/AWS RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white"/> <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/>

### Open API
<img src="https://img.shields.io/badge/TMDB-01D277?style=for-the-badge&logo=themoviedatabase&logoColor=white"/> <img src="https://img.shields.io/badge/Spotify-1DB954?style=for-the-badge&logo=spotify&logoColor=white"/> <img src="https://img.shields.io/badge/국립중앙도서관-A9A9A9?style=for-the-badge&logoColor=white"/> <img src="https://img.shields.io/badge/Naver-03C75A?style=for-the-badge&logo=naver&logoColor=white"/> <img src="https://img.shields.io/badge/Google-4285F4?style=for-the-badge&logo=google&logoColor=white"/> <img src="https://img.shields.io/badge/Kakao-FEE500?style=for-the-badge&logo=kakao&logoColor=black"/>

### 협업 
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/> <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white"/> <img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white"/> <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=white"/>

<br>

## 🧩 ERD 
[![image.png](https://i.postimg.cc/5yDW50BS/image.png)](https://postimg.cc/wR5rg9b1)

<br>

## 🧾 API

### Auth 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| POST | /api/auth/signup | 회원가입 |
| POST | /api/auth/login | 로그인 |
| POST | /api/auth/logout | 로그아웃 |
| POST | /api/auth/reissue | 토큰 재발급 |
| POST | /api/auth/oauth/callback/{provider} | OAuth 콜백 주소 |

### Users 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| GET | /api/users/{userId} | 유저 프로필 조회 |
| GET | /api/users/me | 내 프로필 조회 |
| GET | /api/users/search | 유저 조회 |

### Diaries 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| POST | /api/diaries | 감상일기 등록 |
| PUT | /api/diaries/{diaryId} | 감상일기 수정 |
| DELETE | /api/diaries/{diaryId} | 감상일기 삭제 |
| GET | /api/diaries/search | 감상일기 검색 |
| GET | /api/diaries/{diaryId} | 감상일기 조회 |

### Contents 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| GET | /api/contents/search | 컨텐츠 검색 |
| GET | /api/contents/{contentId} | 컨텐츠 조회 |

### Tags 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| GET | /api/tags | 태그 조회 |

### Comments 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| POST | /api/comments/{diaryId} | 감상일기 댓글 작성 |
| GET | /api/comments/{diaryId} | 감상일기 댓글 조회 |

### Timeline 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| GET | /api/timeline | 타임라인 조회 |

### Follows 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| POST | /api/follows/{followeeId} | 팔로우 |
| DELETE | /api/follows/{followeeId} | 언팔로우 |
| GET | /api/follows/followings | 팔로우 목록 조회 |

### Likes 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| POST | /api/likes/{diaryId} | 좋아요 등록 |
| DELETE | /api/likes/{diaryId} | 좋아요 취소 |
| GET | /api/likes/count | 좋아요 수 단건 조회 |

### Statistics 
| HTTP | URL | 기능 설명 |
| :---: | :--- | :--- |
| GET | /api/statistics/card | 통계 요약(4가지 카드) |
| GET | /api/statistics/monthly-diary-graph | 최근 6개월 감상 수 그래프 |
| GET | /api/statistics/type-distribution | 전체 콘텐츠 타입 분포 |
| GET | /api/statistics/type-graph | 콘텐츠 타입 별 그래프 |
| GET | /api/statistics/genre-graph | 장르 별 그래프 |
| GET | /api/statistics/emotion-graph | 감정 별 그래프 |
| GET | /api/statistics/ott-graph | OTT 별 그래프 |

<br>

## 🌐 시스템 아키텍처
[![siseutem-akitegcheo-seolgye.png](https://i.postimg.cc/VvZLxmj0/siseutem-akitegcheo-seolgye.png)](https://postimg.cc/2LvDvp9C)

<br>

## 💾 주요 기능
| 타임라인 | 콘텐츠 검색 | 감상일기 작성 |
| :---: | :---: | :---: |
| <a href="https://postimg.cc/ykTfjFpy"><img src="https://i.postimg.cc/Dy9t26qH/seukeulinsyas-2025-10-27-180618.png" width="260px"></a> | <a href="https://postimg.cc/fSnXnryw"><img src="https://i.postimg.cc/zv3kWm1R/1.png" width="260px"></a> | <a href="https://postimg.cc/qNMKTnJx"><img src="https://i.postimg.cc/Sxcfc7H3/2.png" width="260px"></a> |
| **감상일기 조회** | **댓글 조회** | **감상 통계** |
| <a href="https://postimg.cc/bSZtnf5x"><img src="https://i.postimg.cc/2ywFPzFK/seukeulinsyas-2025-10-27-180646.png" width="260px"></a> | <a href="https://postimg.cc/tYV6CyWY"><img src="https://i.postimg.cc/BQmBpnvc/seukeulinsyas-2025-10-27-180732.png" width="260px"></a> | <a href="https://postimg.cc/R6f6RLdv"><img src="https://i.postimg.cc/ZRs8Jfyv/3.png" width="260px"></a> |

| 기능 | 설명 |
| --- | --- |
| **콘텐츠 검색** | TMDB, Spotify, 국립중앙도서관 API를 연동하여 영화·음악·책 검색 기능 제공 |
| **감상일기** | 감상일기 등록/수정/삭제, 공개 여부 설정, 태그/OTT 선택 가능 |
| **통계** | 감상 데이터 기반 그래프(월별 감상 수, OTT/장르/감정별 통계) 제공 |
| **소셜** | 팔로우/언팔로우, 타임라인, 좋아요 기능 구현 |
| **인증/인가** | JWT + OAuth(Google, Kakao, Naver) 로그인 구현 |

<br>

## 🔄 개발 프로세스
[👉 개발 및 배포 프로세스 & Git 컨벤션 가이드 바로가기](https://github.com/jueunk617/ourlog-java/wiki/%F0%9F%9A%80-%EA%B0%9C%EB%B0%9C-%EB%B0%8F-%EB%B0%B0%ED%8F%AC-%ED%94%84%EB%A1%9C%EC%84%B8%EC%8A%A4-&-Git-%EC%BB%A4%EB%B2%A4%EC%88%9C-%EC%B0%80%EC%9D%B4%EB%93%9C)

<br>

## 🧠 트러블슈팅

### 1️⃣ [JPA] `NonUniqueObjectException` (영속성 컨텍스트 충돌)

* 💥 **문제:**
    감상일기 수정 시 다대다(M:N) 관계(Tag, Ott) 갱신 과정에서 `NonUniqueObjectException` 발생.
* 🔍 **원인:**
    `list.clear()`로 컬렉션을 비운 뒤 `flush()` 없이 새 엔티티를 `add()` 함. 이로 인해 영속성 컨텍스트 내에 동일 식별자를 가진 객체가 2개(기존, 새 객체) 존재하며 충돌 발생.
* ✅ **해결:**
    * **(1차)** `clear()` 직후 `flush()`를 명시적으로 호출해 삭제 쿼리를 즉시 실행시킴.
    * **(2차 리팩토링)** 비효율적인 '전체 삭제 후 추가' 방식 대신, 기존 목록과 새 목록을 비교해 변경된 항목만 `add`/`remove`하는 **"Delta Update"** 로직으로 개선함.
    * `list.removeAll()`이 정상 동작하도록 연관 엔티티(`Tag`, `Ott` 등)에 `id` 기준 `equals()`와 `hashCode()`를 오버라이딩하여 객체 동등성 비교 문제를 해결함.

<br>

### 2️⃣ [Redis] `ClassCastException` (캐시 역직렬화 오류)

* 💥 **문제:**
    `@Cacheable`로 캐시된 데이터를 조회할 때 `LinkedHashMap cannot be cast to ...Dto` 오류 발생.
* 🔍 **원인:**
    `GenericJackson2JsonRedisSerializer`가 DTO를 JSON으로 직렬화할 때 **타입 정보를 포함하지 않았음.** 이로 인해 역직렬화 시 `LinkedHashMap`으로 변환됨.
* ✅ **해결:**
    * `RedisCacheManager` 설정 시 `ObjectMapper`에 `activateDefaultTyping(...)` 설정을 추가함.
    * JSON 저장 시 `@class` 프로퍼티(예: `"@class": "com.back.ourlog.dto.DiaryDetailDto"`)를 함께 저장하도록 강제하여, 역직렬화 시 명확한 타입으로 복원되도록 수정함.

<br>

### 3️⃣ [API] 프론트엔드-백엔드 데이터 동기화 (ID vs Name)

* 💥 **문제:**
    태그/OTT 수정 시, 프론트엔드에서 보낸 `tagId`가 백엔드 DB에 존재하지 않아 수정이 반영되지 않음.
* 🔍 **원인:**
    프론트엔드가 자체 관리하는 ID와 DB의 Auto-Increment ID가 불일치함.
* ✅ **해결:**
    * API 스펙을 ID 기반에서 **'이름(Name)' 기반**으로 변경함. (ex: `tagNames: ["힐링", "인생영화"]`)
    * 백엔드에서 `findOrCreateTagsByNames()` 메서드를 구현, 받은 이름으로 태그를 조회(Find)하거나 없으면 생성(Create)하도록 로직을 변경함.
    * `GET /api/tags` API를 신설하여 프론트엔드에 DB의 실제 태그 목록을 제공, 데이터 일관성을 확보함.

<br>

### 4️⃣ [외부 API] 응답 구조 파편화 및 데이터 정규화

* 💥 **문제:**
    * TMDB, Spotify, 국립중앙도서관 API의 응답 JSON 구조가 모두 상이하여 공통 처리가 어려웠음.
    * 데이터가 누락되거나(Spotify `track`의 장르), 코드로만 제공됨(TMDB 장르 ID, 도서관 KDC 코드).
    * Spotify DTO 파싱 시, Non-static 중첩 클래스로 인한 `ObjectMapper` 역직렬화 오류 발생.
* ✅ **해결:**
    * **`ContentSearchFacade`** 패턴을 도입, 여러 외부 API의 인터페이스를 단일화함.
    * 각 API별 데이터 정규화 로직을 Facade 하위 서비스에 구현함.
        * **TMDB:** `genreId` ↔ `genreName` 매핑 테이블을 생성해 `{"id": 18}` 같은 숫자 ID를 "드라마" 등 가독성 있는 이름으로 변환.
        * **국립중앙도서관:** `genre` 필드 부재. `kdc`("813.6"), `subject`("한국 소설") 필드를 조합해 "문학", "소설" 등으로 장르명을 역추론.
        * **Spotify:** `track` 조회 시 장르가 없어, `artistId`를 추출해 아티스트 API를 2차 호출해야 장르 정보 획득 가능. (백엔드에서 Client Credentials Flow로 토큰 발급)
    * Spotify DTO의 중첩 클래스를 모두 별도 public 파일로 분리해 `ObjectMapper` 파싱 오류를 해결함.

<br>

### 5️⃣ [TDD] `contextLoads()` 테스트 실패 (`Unable to determine Dialect`)

* 💥 **문제:**
    `@SpringBootTest` 실행 시 `Unable to determine Dialect without JDBC metadata` 오류 발생.
* 🔍 **원인:**
    테스트 컨텍스트 부팅 시 Hibernate가 H2 DB에 연결하지 못해 DB 종류(Dialect) 추론에 실패함.
* ✅ **해결:**
    `application-test.yml`에 `spring.jpa.database-platform: org.hibernate.dialect.H2Dialect` 설정을 명시적으로 추가하여, DB 연결 없이도 Dialect를 인지하도록 함.

<br>

## 💡 주요 결정 및 배운 점

* **JPA 다대다(M:N) 관계 설계**
    * `@ManyToMany` 대신, 중간 엔티티(`DiaryTag`)와 `@IdClass`를 통한 복합키 매핑 방식을 채택했습니다.
    * **(Why?)** 당장의 편의성보다 유지보수성과 확장성(ex) 중간 테이블에 추가 필드가 생기는 경우)을 우선했습니다.

* **엔티티와 서비스의 책임 분리 (SRP)**
    * 'Delta Update' 로직(태그/OTT 수정)을 `Diary` 엔티티가 아닌 `DiaryService`의 책임으로 분리했습니다.
    * **(Why?)** 엔티티는 순수 데이터, 서비스는 `Repository` 접근과 예외 처리를 포함한 비즈니스 로직을 담당하는 도메인 설계 원칙을 적용했습니다.

* **Facade 패턴을 통한 외부 API 추상화**
    * TMDB, Spotify 등 각기 다른 외부 의존성을 `ContentSearchFacade`라는 단일 창구로 추상화했습니다.
    * **(Why?)** `DiaryService`가 외부 API의 복잡성을 알 필요 없이 `facade.search(...)`만 호출하도록 **결합도를 낮췄습니다.**

* **Cache-Aside 전략과 일관성**
    * 자주 조회되는 `getDiaryDetail`에 Redis 캐싱(`@Cacheable`)을 적용했습니다.
    * **(Why?)** 수정(`@CachePut`) 및 삭제(`@CacheEvict`) 시 캐시를 함께 갱신/제거하여 **데이터 일관성을 보장**하는 `Cache-Aside` 전략을 구현했습니다.

* **TDD의 실질적 효용성**
    * 테스트 코드를 먼저 작성하는 과정(TDD)을 통해 `NonUniqueObjectException` 같은 복잡한 JPA 오류나 DTO의 `@Getter` 누락 등을 조기에 발견했습니다.
    * **(Why?)** 테스트는 단순 기능 검증을 넘어, **설계의 문제점을 빠르게 피드백**받는 핵심 도구임을 배웠습니다.
