---
api_specs:
- filename: userback-openapi.yml
  format: yaml
  label: Userback REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userback/refs/heads/main/openapi/userback-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: userback.io
  spf: true
hosts:
- cert_expires: Sep 26 01:50:27 2026 GMT
  host: www.userback.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 28 16:00:34 2026 GMT
  host: docs.userback.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: rest.userback.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Userback Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Userback, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Userback
provider_slug: userback
slug: userback-domain-security
source_filename: userback-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.userback.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 01:50:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.userback.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:00:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.userback.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: userback.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/userback/refs/heads/main/security/userback-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Customer Feedback
- Bug Reporting
- Visual Feedback
- Session Replay
- Product Management
- SaaS
---
