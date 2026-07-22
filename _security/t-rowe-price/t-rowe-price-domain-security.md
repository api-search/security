---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: troweprice.com
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.troweprice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: T Rowe Price Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for T. Rowe Price, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: T. Rowe Price
provider_slug: t-rowe-price
slug: t-rowe-price-domain-security
source_filename: t-rowe-price-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.troweprice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: troweprice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/t-rowe-price/refs/heads/main/security/t-rowe-price-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asset Management
- Investment Management
- Retirement
- Finance
- Mutual Funds
- ETFs
- 401k
- Institutional Investing
- Fortune 1000
---
