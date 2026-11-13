# Taromi hub
Static landing page. Edit `config.js` for people/links. Preview images go in `shots/` (svg/jpg, 16:10).

## Plan
- Repo `taromi-hub` -> main domain (taromi.net / www)
- One repo per person -> own subdomain (fatemeh.taromi.net, mohsen.taromi.net, mahdi.taromi.net)
- GitHub Pages allows ONE custom domain per repo: put a `CNAME` file in each repo with its hostname.

## DNS (after buying the domain)
- A records for apex: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- CNAME `www`, `fatemeh`, `mohsen`, `mahdi` -> <github-user>.github.io
- Then Settings > Pages > Custom domain + Enforce HTTPS.
- Do NOT put mail DNS records (MX/SPF/DKIM) on these subdomains; keep email on the main domain.
