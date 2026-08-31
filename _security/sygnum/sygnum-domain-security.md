---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sygnum.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.sygnum.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: developer.sygnum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 21:50:15 2026 GMT
  host: api.sygnum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sygnum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sygnum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sygnum
provider_slug: sygnum
slug: sygnum-domain-security
source_filename: sygnum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sygnum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.sygnum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: api.sygnum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 21:50:15 2026 GMT\n  hsts: null\ndomains:\n- domain: sygnum.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sygnum/refs/heads/main/security/sygnum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Digital Assets
- Cryptocurrency
- Custody
- Trading
- Staking
- Tokenization
- Settlement
- Market Data
- Financial-Services
- Switzerland
- Singapore
- B2B
---
