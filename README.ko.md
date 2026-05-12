<h1 align="center" style="border-bottom: none">
  <div>
    <a href="https://www.docuseal.com">
      <img  alt="DocuSeal" src="https://github.com/user-attachments/assets/38b45682-ffa4-4919-abde-d2d422325c44" width="80" />
      <br>
    </a>
    DocuSeal
  </div>
</h1>
<h3 align="center">
  오픈소스 문서 작성 및 서명 플랫폼
</h3>
<p align="center">
  <a href="https://hub.docker.com/r/docuseal/docuseal">
    <img alt="Docker releases" src="https://img.shields.io/docker/v/docuseal/docuseal">
  </a>
  <a href="https://discord.gg/qygYCDGck9">
    <img src="https://img.shields.io/discord/1125112641170448454?logo=discord"/>
  </a>
  <a href="https://twitter.com/intent/follow?screen_name=docusealco">
    <img src="https://img.shields.io/twitter/follow/docusealco?style=social" alt="@docusealco 팔로우" />
  </a>
</p>
<p>
DocuSeal은 안전하고 효율적인 디지털 문서 서명 및 처리 기능을 제공하는 오픈소스 플랫폼입니다. PDF 양식을 만들어 사용하기 쉬운 모바일 최적화 웹 도구로 어떤 기기에서든 온라인으로 작성하고 서명할 수 있습니다.
</p>
<h2 align="center">
  <a href="https://demo.docuseal.tech">✨ 라이브 데모</a>
  <span>|</span>
  <a href="https://docuseal.com/sign_up">☁️ 클라우드에서 사용하기</a>
</h2>

[![데모](https://github.com/docusealco/docuseal/assets/5418788/d8703ea3-361a-423f-8bfe-eff1bd9dbe14)](https://demo.docuseal.tech)

## 주요 기능
- PDF 양식 필드 빌더 (WYSIWYG)
- 12가지 필드 유형 지원 (서명, 날짜, 파일, 체크박스 등)
- 문서당 여러 제출자 지원
- SMTP를 통한 자동 이메일 발송
- 디스크, AWS S3, Google Storage, Azure Cloud 파일 저장
- 자동 PDF 전자서명
- PDF 서명 검증
- 사용자 관리
- 모바일 최적화
- 서명 가능 14개 언어를 포함한 7개 UI 언어 지원
- 통합을 위한 API 및 웹훅
- 몇 분 안에 간편하게 배포 가능

## Pro 기능
- 회사 로고 및 화이트라벨
- 사용자 역할 관리
- 자동 리마인더
- SMS를 통한 초대 및 신원 확인
- 조건부 필드 및 수식
- CSV, XLSX 스프레드시트 가져오기를 통한 대량 전송
- SSO / SAML
- HTML API를 이용한 템플릿 생성 ([가이드](https://www.docuseal.com/guides/create-pdf-document-fillable-form-with-html-api))
- PDF 또는 DOCX와 필드 태그 API를 이용한 템플릿 생성 ([가이드](https://www.docuseal.com/guides/use-embedded-text-field-tags-in-the-pdf-to-create-a-fillable-form))
- 임베드 서명 양식 ([React](https://github.com/docusealco/docuseal-react), [Vue](https://github.com/docusealco/docuseal-vue), [Angular](https://github.com/docusealco/docuseal-angular) 또는 [JavaScript](https://www.docuseal.com/docs/embedded))
- 임베드 문서 양식 빌더 ([React](https://github.com/docusealco/docuseal-react), [Vue](https://github.com/docusealco/docuseal-vue), [Angular](https://github.com/docusealco/docuseal-angular) 또는 [JavaScript](https://www.docuseal.com/docs/embedded))
- [자세히 알아보기](https://www.docuseal.com/pricing)

## 배포

|Heroku|Railway|
|:--:|:---:|
| [<img alt="Heroku에 배포" src="https://www.herokucdn.com/deploy/button.svg" height="40">](https://heroku.com/deploy?template=https://github.com/docusealco/docuseal-heroku) | [<img alt="Railway에 배포" src="https://railway.app/button.svg" height="40">](https://railway.com/deploy/IGoDnc?referralCode=ruU7JR)|
|**DigitalOcean**|**Render**|
| [<img alt="DigitalOcean에 배포" src="https://www.deploytodo.com/do-btn-blue.svg" height="40">](https://cloud.digitalocean.com/apps/new?repo=https://github.com/docusealco/docuseal-digitalocean/tree/master&refcode=421d50f53990) | [<img alt="Render에 배포" src="https://render.com/images/deploy-to-render-button.svg" height="40">](https://render.com/deploy?repo=https://github.com/docusealco/docuseal-render)

#### Docker

```sh
docker run --name docuseal -p 3000:3000 -v.:/data docuseal/docuseal
```

기본적으로 DocuSeal Docker 컨테이너는 SQLite 데이터베이스를 사용하여 데이터와 설정을 저장합니다. `DATABASE_URL` 환경 변수를 지정하면 PostgreSQL 또는 MySQL 데이터베이스를 대신 사용할 수 있습니다.

#### Docker Compose

개인 서버에 docker-compose.yml을 다운로드합니다:
```sh
curl https://raw.githubusercontent.com/docusealco/docuseal/master/docker-compose.yml > docker-compose.yml
```

Caddy를 통해 SSL 인증서를 자동 발급하여 사용자 도메인으로 HTTPS 앱을 실행합니다 (DNS가 서버를 가리키고 있어야 합니다):
```sh
sudo HOST=your-domain-name.com docker compose up
```

## 기업을 위한 DocuSeal
### 웹 또는 모바일 앱에 원활한 문서 서명 기능을 통합하세요

DocuSeal은 문서 생성, 작성, 서명 및 처리를 여러분의 제품과 원활하게 통합하기 위한 전문성과 기술을 보유하고 있습니다. **금융, 의료, 운송, 부동산, 이커머스, KYC, CRM 등 대량 문서 서명이 필요한 다양한 산업**과의 협업을 전문으로 합니다. DocuSeal을 활용하여 전자 문서의 개발 및 처리 비용을 절감하는 동시에 보안과 현지 전자문서 법규 준수를 보장합니다.

[미팅 예약하기](https://www.docuseal.com/contact)

## 라이선스

Section 7(b) 추가 조항이 포함된 AGPLv3 라이선스 하에 배포됩니다. 자세한 내용은 [LICENSE](https://github.com/docusealco/docuseal/blob/master/LICENSE) 및 [LICENSE_ADDITIONAL_TERMS](https://github.com/docusealco/docuseal/blob/master/LICENSE_ADDITIONAL_TERMS)를 참조하세요.
별도의 명시가 없는 한, 모든 파일의 저작권은 © 2023-2026 DocuSeal LLC에 있습니다.

## 관련 도구

- [온라인 서명 만들기](https://www.docuseal.com/online-signature)
- [온라인 문서 서명](https://www.docuseal.com/sign-documents-online)
- [온라인 PDF 작성](https://www.docuseal.com/fill-pdf)
