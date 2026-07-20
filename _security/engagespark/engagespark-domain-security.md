---
api_specs:
- filename: engagespark-openapi-original.yml
  format: yaml
  label: engageSPARK API
  slug: engagespark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagespark/refs/heads/main/openapi/engagespark-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: engagespark.com
  spf: true
hosts:
- cert_expires: Oct  9 19:56:28 2026 GMT
  host: engagespark.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 06:41:05 2026 GMT
  host: openapi.engagespark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 04:09:15 2026 GMT
  host: api.engagespark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Engagespark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for engageSPARK, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: engageSPARK
provider_slug: engagespark
slug: engagespark-domain-security
source_filename: engagespark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: engagespark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 19:56:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: openapi.engagespark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:41:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.engagespark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:09:15 2026 GMT\n  hsts: null\ndomains:\n- domain: engagespark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engagespark/refs/heads/main/security/engagespark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Messaging
- SMS
- Voice
- WhatsApp
- Airtime
- Communications
- CPaaS
- Surveys
- International Development
---
