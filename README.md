# 🌐 언제더라 (WhenDidI) - Landing Page

이 폴더는 **언제더라** 앱의 랜딩 페이지입니다.

## 📁 Repository 구조

| 저장소 | 타입 | URL |
|:---|:---:|:---|
| **Landing Page (WEB)** | Public | https://github.com/proxima-e/-When-Did-I-WEB |
| **App (Main)** | Private | https://github.com/proxima-e/-WhenDidI- |

---

## 🚀 커밋 & 푸시 방법

### WEB 변경사항만 푸시할 때
```bash
cd WEB
git add .
git commit -m "커밋 메시지"
git push origin main
```

### 자동화된 푸시 요청 (Claude에게)
```
"WEB 변경사항 커밋/푸시해줘" 라고 요청하면:
1. WEB 저장소에 먼저 푸시 (Public)
2. 앱 저장소의 서브모듈 참조 업데이트 (Private)
```

---

## 📝 파일 설명

| 파일 | 설명 |
|:---|:---|
| `index.html` | 현재 배포 중인 랜딩 페이지 (최소 버전) |
| `_backup.html` | 출시 후 사용할 전체 기능 버전 |
| `style.css` | 스타일시트 |
| `SEO_GUIDE.md` | SEO 최적화 가이드 |
| `assets/` | 이미지 및 리소스 |

---

## 🔗 배포 URL

**GitHub Pages**: https://proxima-e.github.io/-When-Did-I-WEB/

---

© 2026 Proxima. All rights reserved.
