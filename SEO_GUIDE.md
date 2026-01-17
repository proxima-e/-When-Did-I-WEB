# 언제더라(WhenDidI) 웹페이지 SEO 및 노션 연동 가이드

이 문서는 생성된 `WEB` 폴더의 소개 페이지를 인터넷에 배포하고, 검색 엔진에 노출시키며, 노션에 연동하는 방법을 안내합니다.

## 1. 웹사이트 무료 호스팅 (배포하기)
웹페이지(`index.html`)를 인터넷 주소(URL)로 접속할 수 있게 하려면 '호스팅'이 필요합니다. **GitHub Pages**를 추천합니다.

1.  GitHub 저장소에 `WEB` 폴더의 내용이 푸시(업로드)되어 있어야 합니다.
2.  GitHub 저장소 설정(Settings) -> **Pages** 메뉴로 이동합니다.
3.  Source를 `Deploy from a branch`로 선택합니다.
4.  Branch를 `main` (또는 현재 브랜치)로 선택하고, 폴더를 `/` (root) 대신 `/WEB`으로 설정할 수 있다면 좋겠지만, GitHub Pages는 보통 루트나 `/docs`만 지원합니다.
    *   **방법**: 현재 `WEB` 폴더의 내용물(`index.html`, `style.css`, `assets`)을 저장소의 루트로 옮기거나, `docs`라는 이름으로 폴더명을 변경하고 GitHub Pages 설정에서 `/docs`를 선택하면 됩니다.
5.  Save를 누르면 몇 분 후 `https://사용자명.github.io/저장소명/` 주소가 생성됩니다.

## 2. 노션(Notion)에 웹페이지 올리기
노션은 HTML 파일을 직접 업로드해서 보여주는 기능은 없지만, **위에서 만든 URL을 임베드**할 수 있습니다.

### 방법 A: 임베드 (Embed)
웹페이지를 노션 안에서 바로 보여줍니다.
1.  노션 페이지에서 `/embed` 입력 후 엔터.
2.  위에서 생성한 GitHub Pages URL (예: `https://proxima-e.github.io/-WhenDidI-`)을 입력.
3.  웹사이트가 노션 페이지 안에 작은 창으로 나타납니다.

### 방법 B: 북마크 또는 링크
1.  URL을 붙여넣고 '북마크 생성'을 선택하면 예쁜 썸네일과 함께 링크가 생성됩니다.

## 3. SEO (검색 엔진 최적화) 가이드
구글 검색에 노출되려면 **Google Search Console**에 사이트를 등록해야 합니다.

1.  [Google Search Console](https://search.google.com/search-console) 접속.
2.  'URL 접두어' 방식 선택 후 웹사이트 URL 입력.
3.  소유권 확인:
    *   HTML 파일 업로드 방식을 선택하면 확인용 파일을 줍니다.
    *   이 파일을 `WEB` 폴더에 넣고 다시 GitHub에 푸시/배포합니다.
    *   확인 버튼을 누르면 등록 완료.
4.  **Sitemap 제출**:
    *   사이트가 단순하므로 필수는 아니지만, `sitemap.xml`을 만들어 제출하면 더 좋습니다.

### 메타 태그 최적화
현재 `index.html`에 이미 기본적인 메타 태그가 적용되어 있습니다.
```html
<meta name="description" content="설명...">
<meta name="keywords" content="키워드...">
<meta property="og:title" content="...">
```
이 내용을 앱의 특징에 맞게 주기적으로 업데이트해주면 검색 노출에 도움이 됩니다.
