---
api_specs:
- filename: index.html
  format: yaml
  label: Small Improvements REST API
  slug: small-improvements-rest-api
  spec_type: OpenAPI
  url: https://storage.googleapis.com/si-rest-api-docs/dist/index.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: small-improvements.com
  spf: true
hosts:
- cert_expires: Sep  4 22:29:07 2026 GMT
  host: www.small-improvements.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:21:32 2026 GMT
  host: intercomdocs.small-improvements.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 28 23:59:59 2027 GMT
  host: app.small-improvements.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Small Improvements Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Small Improvements, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Small Improvements
provider_slug: small-improvements
slug: small-improvements-domain-security
source_filename: small-improvements-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.small-improvements.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:29:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: intercomdocs.small-improvements.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.small-improvements.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: small-improvements.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/small-improvements/refs/heads/main/security/small-improvements-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Performance Management
- HR
- Employee Feedback
- OKRs
- 1:1 Meetings
- Pulse Surveys
- 360 Feedback
- People Management
---
