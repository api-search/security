---
api_specs:
- filename: uplimit-course-api-openapi.yml
  format: yaml
  label: Uplimit Course API
  slug: uplimit-course-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplimit/refs/heads/main/openapi/uplimit-course-api-openapi.yml
- filename: uplimit-export-api-openapi.yml
  format: yaml
  label: Uplimit Export API
  slug: uplimit-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplimit/refs/heads/main/openapi/uplimit-export-api-openapi.yml
- filename: uplimit-platform-api-openapi.yml
  format: yaml
  label: Uplimit Platform API
  slug: uplimit-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplimit/refs/heads/main/openapi/uplimit-platform-api-openapi.yml
- filename: uplimit-session-api-openapi.yml
  format: yaml
  label: Uplimit Session API
  slug: uplimit-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplimit/refs/heads/main/openapi/uplimit-session-api-openapi.yml
- filename: uplimit-user-api-openapi.yml
  format: yaml
  label: Uplimit User API
  slug: uplimit-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uplimit/refs/heads/main/openapi/uplimit-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uplimit.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: uplimit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uplimit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uplimit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Uplimit
provider_slug: uplimit
slug: uplimit-domain-security
source_filename: uplimit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uplimit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: uplimit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplimit/refs/heads/main/security/uplimit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Future Of Work
- Learning
- Education
- Training
- Artificial Intelligence
- Corporate Training
---
