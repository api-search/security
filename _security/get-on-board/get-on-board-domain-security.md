---
api_specs:
- filename: get-on-board-openapi-original.yml
  format: yaml
  label: Get on Board API
  slug: get-on-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/get-on-board/refs/heads/main/openapi/get-on-board-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getonbrd.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: getonbrd.dev
  spf: false
hosts:
- cert_expires: Sep 29 07:53:31 2026 GMT
  host: getonbrd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 07:53:31 2026 GMT
  host: www.getonbrd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 04:16:13 2026 GMT
  host: sandbox.getonbrd.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Get On Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Get On Board, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Get On Board
provider_slug: get-on-board
slug: get-on-board-domain-security
source_filename: get-on-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getonbrd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:53:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.getonbrd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:53:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.getonbrd.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 04:16:13 2026 GMT\n  hsts: false\ndomains:\n- domain: getonbrd.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getonbrd.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/get-on-board/refs/heads/main/security/get-on-board-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Recruitment
- Jobs
- Hiring
- ATS
- Talent
- Developers
- Latin America
---
