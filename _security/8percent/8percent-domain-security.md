---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 8percent.kr
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: 8percent.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: core-api.8percent.kr
  hsts: false
  https: true
  note: JSON API host for the consumer app; GET /health returns 200 application/json
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: api.8percent.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: loan.8percent.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: events.8percent.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: about.8percent.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: blog.8percent.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 7
kind: domain-security
layout: security
method: probed
name: 8Percent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 8percent, probed live across 7 host(s) and 1 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 8percent
provider_slug: 8percent
slug: 8percent-domain-security
source_filename: 8percent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the 8percent.kr registrable domain and every first-party\n  host named in the 8percent.kr production JavaScript bundle (/assets/index-DenshHdQ.js)\nnotes: >-\n  Every first-party host terminates TLS 1.3 with a valid certificate, but not one of them\n  returns a Strict-Transport-Security header — including core-api.8percent.kr, the JSON API\n  host the consumer app calls. The 8percent.kr zone is not DNSSEC-signed and publishes no CAA\n  record, so certificate issuance is unconstrained. SPF and DMARC are both published, with\n  DMARC at p=quarantine.\nhosts:\n- host: 8percent.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\n- host: core-api.8percent.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\n  note: JSON API host for the consumer app; GET /health returns 200 application/json\n- host: api.8percent.kr\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\n- host: loan.8percent.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\n- host: events.8percent.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\n- host: about.8percent.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\n- host: blog.8percent.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 8percent.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/8percent/refs/heads/main/security/8percent-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- P2P Lending
- Marketplace Lending
- Credit Scoring
- Investing
- Consumer Finance
- Real Estate Lending
- Tokenization
- South Korea
---
