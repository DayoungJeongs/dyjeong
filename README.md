# Dayoung Jeong — Academic Website

Static HTML/CSS website deployed to https://dyjeong.com/ with GitHub Pages.

- index.html is the complete profile homepage. It requires no JavaScript to read the biography, research interests, contact details, or navigation.
- home.html retains the same profile for existing external links, with canonical https://dyjeong.com/. Keep it synchronized with index.html when updating the profile.
- Internal Home and site-name links point to /.
- sitemap.xml lists the canonical homepage, research.html, teaching.html, and the public CV PDF. Do not add the duplicate home.html.
- robots.txt explicitly permits OAI-SearchBot, Googlebot, Bingbot, ChatGPT-User, and all other crawlers. GPTBot retains the previous allow policy, stated separately from search access.
- ProfilePage/Person structured data is included in both profile documents, with bilingual identity, verified official profiles, affiliation, and ORCID.
- research.html includes 56 ScholarlyArticle records matching its existing titles and English abstracts. DOI identifiers are supplied for the 45 records with verified DOIs; the remaining records retain KCI identifiers.
- Optional citation downloads and DBpia linking are deferred by the owner. No visible content, navigation, CSS, or page structure changed in this SEO update.
- The four canonical sitemap URLs are retained. HTML lastmod dates reflect the 2026-10-03 metadata update. home.html remains excluded as a duplicate.
- No new Research Agenda, navigation item, individual article page, working-paper page, or tracking script was added in this SEO update.
- The former signature intro is archived outside the deployed site in both the academic and cultural website workspaces, under _서명인트로_보관/2026-09-26_원본. See 복원방법.md there before restoring or reusing it.
- CV remains cv/Dayoung_Jeong_CV.pdf. Assets and styling are unchanged.

Deploy the repository root from the main branch with GitHub Pages. CNAME belongs to dyjeong.com.
