# HTTP 보안 헤더 완전 레퍼런스

OWASP HTTP Headers Cheat Sheet, MDN Web Docs, PortSwigger Web Security Academy를 기준으로 정리한 HTTP 보안 헤더 레퍼런스 페이지입니다. Burp Suite 화면을 재현한 예시로 실전 진단 방법까지 함께 다룹니다.

🔗 **[페이지 바로가기](https://zz1231me.github.io/http-security-headers-guide/)**

## 다루는 내용

- **Burp Suite 실전 분석** — HTTP History·Repeater 화면 재현, 취약한 응답 vs 안전한 응답 비교
- **필수 보안 헤더 8종** — CSP, HSTS, X-Frame-Options, X-Content-Type-Options, Referrer-Policy, Permissions-Policy, Cache-Control, Content-Type
- **Cross-Origin 헤더 5종** — CORS, COOP·COEP·CORP, Sec-Fetch-*(Fetch Metadata)
- **정보 노출·유틸리티 헤더 9종** — Server, X-Powered-By, X-AspNet-Version, Set-Cookie, Clear-Site-Data, Secure File Download, X-Permitted-Cross-Domain-Policies, X-Robots-Tag, X-DNS-Prefetch-Control
- **Deprecated 헤더 4종** — X-XSS-Protection, Expect-CT, HPKP, FLoC
- **진단 체크리스트 & 공격 유형 → 방어 헤더 매핑표**
- **일반 HTTP 헤더 참고표** — 보안과 무관하지만 실무에서 자주 보이는 Host, Accept, ETag, Cache-Control, X-Forwarded-*, Authorization 등을 카테고리별 표로 정리

각 헤더 카드는 개요, 취약점 도출, Burp 실전 코드, 서버별(Apache/Nginx/Express/PHP 등) 설정 예시 탭으로 구성되어 있습니다. 본문 폰트는 Google Fonts의 Noto Sans KR, 코드 블록은 JetBrains Mono를 사용합니다.

## 로컬에서 보기

별도 빌드 과정 없이 순수 HTML/CSS/JS로만 작성되어 있습니다. `index.html`을 브라우저로 열면 바로 확인할 수 있습니다.

```bash
open index.html   # macOS
```

## 출처

- [OWASP HTTP Headers Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/HTTP_Headers_Cheat_Sheet.html)
- [MDN Web Docs — HTTP Headers](https://developer.mozilla.org/ko/docs/Web/HTTP/Headers)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)
