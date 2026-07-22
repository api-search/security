---
api_specs:
- filename: yoobic-openapi.json
  format: json
  label: YOOBIC Public API
  slug: yoobic-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoobic/refs/heads/main/openapi/yoobic-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yoobic.com
  spf: true
hosts:
- cert_expires: Sep 29 12:12:47 2026 GMT
  host: www.yoobic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yoobic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yoobic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yoobic
provider_slug: yoobic
slug: yoobic-domain-security
source_filename: yoobic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yoobic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: yoobic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoobic/refs/heads/main/security/yoobic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Frontline Operations
- Task Management
- Workforce
- Microlearning
- Employee Experience
- REST
- Webhooks
- SCIM
---
