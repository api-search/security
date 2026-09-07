---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ababa.co.jp
  spf: false
hosts:
- cert_expires: Oct  7 20:32:24 2026 GMT
  host: hr.ababa.co.jp
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 07:33:30 2026 GMT
  host: ababa.co.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 'Bubble.io-hosted end-user application behind Cloudflare; robots.txt is Disallow: / for all user agents.'
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: api.ababa.co.jp
  hsts: false
  hsts_max_age: null
  https: true
  note: 'First-party API host (AWS ap-northeast-1). Answers 404 text/plain at the root with permissive CORS (access-control-allow-origin: *, X-Acting-Company-ID); /health returns 200 application/json. No HSTS header. Undocumented: no portal, reference or specification is published for it.'
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ababa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ABABA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ABABA
provider_slug: ababa
slug: ababa-domain-security
source_filename: ababa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the ababa.co.jp application\n  host and the api.ababa.co.jp first-party API host found by DNS\nhosts:\n- host: hr.ababa.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:32:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: ababa.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 07:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: 'Bubble.io-hosted end-user application behind Cloudflare; robots.txt is Disallow:\n    / for all user agents.'\n- host: api.ababa.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n  note: 'First-party API host (AWS ap-northeast-1). Answers 404 text/plain at the\n    root with permissive CORS (access-control-allow-origin: *, X-Acting-Company-ID);\n    /health returns 200 application/json. No HSTS header. Undocumented:\
  \ no portal,\n    reference or specification is published for it.'\ndomains:\n- domain: ababa.co.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ababa/refs/heads/main/security/ababa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Human Resources
- Recruiting
- Talent Acquisition
- HR Technology
- Job Search
- Artificial Intelligence
- Japan
- SaaS
---
