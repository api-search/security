---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hakimo.ai
  spf: true
hosts:
- cert_expires: Nov 10 02:53:16 2026 GMT
  host: www.hakimo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 15:15:00 2026 GMT
  cert_issuer: Google Trust Services WE1
  host: portal.hakimo.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Customer application portal (Angular SPA). Its tenant API is served same-origin under /v2/orm/ and answers unauthenticated requests with HTTP 401 {"message":"Invalid token"}.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hakimo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hakimo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hakimo
provider_slug: hakimo
slug: hakimo-domain-security
source_filename: hakimo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hakimo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 02:53:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.hakimo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:15:00 2026 GMT\n  cert_issuer: Google Trust Services WE1\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Customer application portal (Angular SPA). Its tenant API is served same-origin under\n    /v2/orm/ and answers unauthenticated requests with HTTP 401 {\"message\":\"Invalid token\"}.\ndomains:\n- domain: hakimo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hakimo/refs/heads/main/security/hakimo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical Security
- Video Surveillance
- Access Control
- Artificial Intelligence
- Computer Vision
- Security Operations
- Remote Guarding
- Alarm Monitoring
- Facility Management
---
