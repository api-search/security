---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coinnudge.site
  spf: true
hosts:
- cert_expires: Dec  4 10:42:49 2026 GMT
  host: coinnudge.site
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coinnudge Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinNudge API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CoinNudge API
provider_slug: coinnudge-api
slug: coinnudge-api-domain-security
source_filename: coinnudge-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinnudge.site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 10:42:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coinnudge.site\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinnudge-api/refs/heads/main/security/coinnudge-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cryptocurrency
- Market Data
- Trading
- Quantitative Finance
- Research
- Derivatives
- Financial Data
- Datasets
---
