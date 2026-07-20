---
api_specs:
- filename: go1-openapi.yml
  format: yaml
  label: Go1 API
  slug: go1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/openapi/go1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: go1.com
  spf: true
hosts:
- cert_expires: Sep 14 21:00:56 2026 GMT
  host: www.go1.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 21:00:56 2026 GMT
  host: developers.go1.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 21:00:56 2026 GMT
  host: gateway.go1.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Go1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Go1, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Go1
provider_slug: go1
slug: go1-domain-security
source_filename: go1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.go1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:00:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.go1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:00:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: gateway.go1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:00:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: go1.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go1/refs/heads/main/security/go1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Edtech
- Learning
- E-Learning
- Corporate Training
- Content
- Learning Management
- LMS
- Education
- Webhooks
---
