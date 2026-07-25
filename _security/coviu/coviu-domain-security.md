---
api_specs:
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Sessions API
  slug: coviu-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Participants API
  slug: coviu-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Waiting Area API
  slug: coviu-waiting-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Collections API
  slug: coviu-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
- filename: coviu-rest-api-openapi.json
  format: json
  label: Coviu Webhooks
  slug: coviu-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-rest-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coviu.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.coviu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: coviu.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: api.coviu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coviu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coviu, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coviu
provider_slug: coviu
slug: coviu-domain-security
source_filename: coviu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coviu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: coviu.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coviu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: coviu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/security/coviu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Telehealth
- Australia
- Virtual Care
- Video
- WebRTC
- Appointments
- Remote Monitoring
- REST
---
