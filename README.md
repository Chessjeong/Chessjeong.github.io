# Minho Jeong · Academic Homepage

[luost26/academic-homepage](https://github.com/luost26/academic-homepage)를 기반으로 만든 Jekyll 홈페이지입니다. 원본 MIT 라이선스와 하단 출처 표기를 유지합니다.

## 로컬 미리보기

Ruby 3.3과 Bundler를 사용합니다. 이 Mac에는 Homebrew Ruby 3.3을 설치해 두었습니다.

```bash
export PATH="/opt/homebrew/opt/ruby@3.3/bin:$PATH"
bundle install
bundle exec jekyll serve --host 127.0.0.1 --port 4000 --livereload
```

브라우저에서 http://127.0.0.1:4000 에 접속합니다. 설정 파일을 바꾸면 서버를 재시작합니다.

## 내용 수정

| 내용 | 파일 |
| --- | --- |
| 소개, 연락처, 사진, 학력, 경력, 교육, 수상 | `_data/profile.yml` |
| 출판된 논문 및 공개 프리프린트 | `_publications/2026/` |
| 심사 중 원고 | `_data/manuscripts.yml` |
| 프로젝트 | `_data/projects.yml` |
| 상단 메뉴 | `_data/navigation.yml` |
| CV PDF | `assets/files/minho-jeong-cv.pdf` |
| 추가 스타일 | `assets/css/custom.css` |
| 도메인과 경로 | `_config.yml` |

논문을 추가하려면 `_publications/2026/2026-causilo.md` 형식으로 Markdown 파일을 만들면 됩니다. `selected: true`인 논문은 첫 화면에도 나타납니다. 저자 이름이 `Minho Jeong` 또는 `M. Jeong`이면 자동으로 강조합니다. 심사 중 원고는 별도 섹션에 표시합니다.

본문과 서지정보의 출처 및 편집 기준은 `docs/content-sources.md`에 기록했습니다. 이 문서는 웹사이트에 포함되지 않습니다. 템플릿 예시 논문·뉴스·블로그·쇼케이스 콘텐츠는 제거했습니다.

## GitHub Pages 배포

- 저장소: https://github.com/Chessjeong/Chessjeong.github.io
- 홈페이지: https://chessjeong.github.io
- 배포 브랜치: `main`
- 배포 방식: GitHub Actions (`.github/workflows/pages.yml`)

`main`에 변경 사항을 푸시하면 자동으로 빌드 후 배포합니다. PR에서는 빌드만 확인합니다. 수동 재배포는 **Actions → Build and deploy academic homepage → Run workflow**에서 `main`을 선택합니다.

워크플로는 Ruby 3.3으로 직접 빌드하므로 원본의 `jekyll-email-protect` 플러그인도 유지됩니다. 원본 템플릿은 `upstream`, 실제 홈페이지 저장소는 `origin` remote로 등록되어 있습니다.

개인 도메인을 사용할 경우 `_config.yml`의 `url`을 수정하고 GitHub Pages의 Custom domain 설정을 적용합니다. 프로젝트 저장소에 배포할 경우 `baseurl`도 저장소 이름에 맞게 바꿉니다.

## 빌드 확인

```bash
bundle exec jekyll build --trace
```

`Gemfile.lock`을 포함해 의존성 버전을 고정했습니다. `_site`, `vendor`, `.bundle`, 문서와 개발 스크립트는 배포 결과에서 제외됩니다.
