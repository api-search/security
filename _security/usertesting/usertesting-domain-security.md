---
api_specs:
- filename: usertesting-clip-api-openapi.yml
  format: yaml
  label: UserTesting Clip API
  slug: usertesting-clip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-clip-api-openapi.yml
- filename: usertesting-general-session-data-api-openapi.yml
  format: yaml
  label: UserTesting General Session Data API
  slug: usertesting-general-session-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-general-session-data-api-openapi.yml
- filename: usertesting-highlightreel-api-openapi.yml
  format: yaml
  label: UserTesting Highlightreel API
  slug: usertesting-highlightreel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-highlightreel-api-openapi.yml
- filename: usertesting-qxscore-data-api-openapi.yml
  format: yaml
  label: UserTesting QXscore Data API
  slug: usertesting-qxscore-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-qxscore-data-api-openapi.yml
- filename: usertesting-session-api-openapi.yml
  format: yaml
  label: UserTesting Session API
  slug: usertesting-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-session-api-openapi.yml
- filename: usertesting-studies-api-openapi.yml
  format: yaml
  label: UserTesting Studies API
  slug: usertesting-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-studies-api-openapi.yml
- filename: usertesting-video-data-api-openapi.yml
  format: yaml
  label: UserTesting Video Data API
  slug: usertesting-video-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-video-data-api-openapi.yml
- filename: usertesting-workspaces-api-openapi.yml
  format: yaml
  label: UserTesting Workspaces API
  slug: usertesting-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-workspaces-api-openapi.yml
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
