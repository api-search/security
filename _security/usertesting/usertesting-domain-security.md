---
api_specs:
- filename: usertesting-results-v2-openapi.yml
  format: yaml
  label: UserTesting Results API (v2)
  slug: usertesting-results-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-results-v2-openapi.yml
- filename: usertesting-legacy-v1-openapi.yml
  format: yaml
  label: UserTesting Legacy API (v1)
  slug: usertesting-legacy-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-legacy-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usertesting.com
  spf: true
hosts:
- cert_expires: Nov  7 09:30:27 2026 GMT
  host: www.usertesting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 10 05:03:23 2026 GMT
  host: developer.usertesting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.use2.usertesting.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usertesting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UserTesting, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UserTesting
provider_slug: usertesting
slug: usertesting-domain-security
source_filename: usertesting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usertesting.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 09:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.usertesting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 05:03:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.use2.usertesting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: usertesting.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/security/usertesting-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- UX Research
- Usability Testing
- Human Insight
- Customer Experience
- Surveys
- Video
- Transcripts
- Experience Metrics
---
