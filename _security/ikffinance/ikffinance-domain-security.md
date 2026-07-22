---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ikffinance.com
  spf: true
hosts:
- cert_expires: Aug 25 11:09:37 2026 GMT
  host: ikffinance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ikffinance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IKF Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IKF Finance
provider_slug: ikffinance
slug: ikffinance-domain-security
source_filename: ikffinance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ikffinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:09:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ikffinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikffinance/refs/heads/main/security/ikffinance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- NBFC
- Lending
- Asset Finance
- Vehicle Finance
- MSME
- India
---
