# Dayoung Jeong — Personal Academic Website

This folder contains a complete, static website (plain HTML + CSS, no build step,
no frameworks, no external CDN resources). It is ready to be uploaded as-is to a
GitHub repository and served with GitHub Pages.

## Deploy with GitHub Pages

1. Create a new GitHub repository (public).
2. Upload the entire contents of this `site` folder to the root of that repository
   (i.e. `index.html`, `style.css`, `CNAME`, `assets/`, etc. should sit at
   the repo root — not inside a subfolder).
3. In the repository, go to **Settings → Pages**, and under "Build and deployment"
   set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. The `CNAME` file already contains `dyjeong.com`. This domain must be
   purchased at a registrar before use. Once purchased, add the corresponding
   DNS records at the registrar (an `A` record set pointing to GitHub Pages'
   IP addresses, or a `CNAME` record if using a subdomain) as described in
   GitHub's custom domain documentation. `dayoungjeong.com` (already owned)
   can be pointed at the same site or set up to redirect to `dyjeong.com`.
5. The "CV" link in the navigation points directly to `cv/Dayoung_Jeong_CV.pdf`
   (no on-page CV — she decided PDF-only is simpler). To update it, edit the
   source docx and regenerate the PDF (see the docx build script used to
   produce it, kept outside this folder), then replace this file.
6. To change the photo, replace `assets/photo.jpg` (or edit the `src`
   attribute in `home.html`).
7. `index.html` is a minimal script-drawn-name "splash" landing page (just
   her name in a cursive font, linking to `home.html`); `home.html` is the
   actual homepage content (photo, bio, contact). All internal navigation
   (site name, "Home" links) points to `home.html`, not `index.html` — this
   is intentional, so visitors only see the splash once on first arrival.

No build tools, package managers, or external fonts/scripts are required; the
site works by simply opening `index.html` in a browser or hosting the folder on
any static file host.

---

## 한국어 배포 안내

이 폴더에는 순수 HTML과 CSS로만 제작된 정적 웹사이트가 들어 있습니다. 별도의
빌드 과정이나 외부 프레임워크, CDN 리소스를 전혀 사용하지 않으므로, 이 폴더를
그대로 GitHub 저장소에 올려 GitHub Pages로 바로 배포할 수 있습니다.

### GitHub Pages로 배포하는 방법

1. GitHub에서 새 저장소(공개 저장소)를 만듭니다.
2. 이 `site` 폴더 안의 모든 파일(`index.html`, `style.css`, `CNAME`, `assets/`
   등)을 저장소의 최상위 경로에 그대로 업로드합니다. (하위 폴더 안에
   넣지 않도록 주의하세요.)
3. 저장소의 **Settings → Pages** 메뉴에서 "Build and deployment" 항목의 소스를
   **Deploy from a branch**, 브랜치 `main`, 폴더 `/ (root)`로 설정합니다.
4. `CNAME` 파일에는 `dyjeong.com`이 기재되어 있습니다. 이 도메인은 아직
   구매 전이므로, 도메인 등록기관(가비아, 후이즈, Namecheap 등)에서 먼저
   구매해야 합니다. 구매 후 GitHub Pages 안내에 따라 DNS 레코드(A 레코드
   또는 서브도메인의 경우 CNAME 레코드)를 설정하세요. 이미 보유 중인
   `dayoungjeong.com`은 같은 사이트로 연결하거나 `dyjeong.com`으로
   자동 리다이렉트되도록 설정할 수 있습니다.
5. 상단 메뉴의 "CV" 링크는 `cv/Dayoung_Jeong_CV.pdf`로 바로 연결됩니다
   (화면용 CV 페이지는 없앴습니다 — PDF 하나로 통일하는 게 더 낫다고
   판단하셨습니다). 내용을 갱신하려면 원본 워드 파일을 수정하고 PDF로
   다시 변환한 뒤 이 파일을 교체하세요.
6. 사진을 바꾸려면 `assets/photo.jpg`를 교체하거나 `home.html`의 `src`
   속성을 수정하세요.
7. `index.html`은 이름만 필기체로 보여주는 인트로(스플래시) 화면이고,
   실제 홈 내용(사진·소개·연락처)은 `home.html`에 있습니다. 사이트 이름과
   "Home" 메뉴는 모두 `home.html`로 연결되도록 해 두었습니다 — 방문자가
   처음 들어올 때만 인트로를 보고, 이후에는 바로 홈으로 이동하게 하기
   위함입니다.

별도의 빌드 도구나 패키지 매니저, 외부 폰트/스크립트가 필요하지 않으므로,
`index.html`을 브라우저에서 바로 열거나 어떤 정적 파일 호스팅 서비스에
올려도 정상적으로 동작합니다.
