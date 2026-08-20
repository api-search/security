---
api_specs:
- filename: banzai-events-api-openapi.yml
  format: yaml
  label: Banzai Events API
  slug: banzai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banzai/refs/heads/main/openapi/banzai-events-api-openapi.yml
- filename: banzai-intro-api-openapi.yml
  format: yaml
  label: Banzai Intro API
  slug: banzai-intro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banzai/refs/heads/main/openapi/banzai-intro-api-openapi.yml
- filename: banzai-reports-api-openapi.yml
  format: yaml
  label: Banzai Reports API
  slug: banzai-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banzai/refs/heads/main/openapi/banzai-reports-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: banzai.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: demio.com
  spf: true
hosts:
- cert_expires: Oct  5 22:59:36 2026 GMT
  host: www.banzai.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 17:44:37 2026 GMT
  host: www.demio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: my.demio.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: API host (baseURL https://my.demio.com/api/v1). Probed manually on 2026-08-06 — GET /api/v1/ping returned HTTP 401 with the HSTS header above.
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: publicdemioapi.docs.apiary.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Banzai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banzai, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Banzai
provider_slug: banzai
slug: banzai-domain-security
source_filename: banzai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.banzai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:59:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.demio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 17:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.demio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    API host (baseURL https://my.demio.com/api/v1). Probed manually on 2026-08-06 —\n    GET /api/v1/ping returned HTTP 401 with the HSTS header above.\n- host: publicdemioapi.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: banzai.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n- domain: demio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banzai/refs/heads/main/security/banzai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketing
- Marketing Technology
- Event Management
- Webinars
- Video
- Engagement Marketing
- Demand Generation
- Software-as-a-Service
---
