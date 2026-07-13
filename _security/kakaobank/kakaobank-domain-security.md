---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kakaobank.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.kakaobank.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: eng.kakaobank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.kakaobank.com
  https: false
kind: domain-security
layout: security
method: probed
name: Kakaobank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KakaoBank, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: KakaoBank
provider_slug: kakaobank
slug: kakaobank-domain-security
source_filename: kakaobank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kakaobank.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: eng.kakaobank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kakaobank.com\n  https: false\ndomains:\n- domain: kakaobank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kakaobank/refs/heads/main/security/kakaobank-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Banking
- Finance
- Open Banking
- Korea
- Fintech
- Account Management
- Transfers
- Loans
- Credit Scoring
- Mobile Banking
---
