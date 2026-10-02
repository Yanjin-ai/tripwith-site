# tripwith-site

Tripwith（同行）的公开站点。GitHub Pages 从 `main` 分支根目录发布。

- `index.html` 首页
- `privacy.html` 隐私政策（英 / 中）
- `.well-known/apple-app-site-association` Universal Link 配置：`https://<域名>/join/<token>` 直接打开 App
- `404.html` 没装 App 的人点邀请链接落到这里（GitHub Pages 没有动态路由，靠 404 接 `/join/*`）
- `.nojekyll` 让 Pages 原样发布 `.well-known` 这种点开头的目录

域名绑定：仓库 Settings → Pages → Custom domain 填域名，再在注册商加 DNS（见主仓库 `docs/真机测试.md`）。
没绑域名前通过 `https://yanjin-ai.github.io/tripwith-site/` 访问——但 Universal Link 必须在自己的域名根路径下才生效。
