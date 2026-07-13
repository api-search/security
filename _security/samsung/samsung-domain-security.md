---
api_specs:
- filename: samsung-smartthings-openapi.yml
  format: yaml
  label: SmartThings API
  slug: smartthings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samsung/refs/heads/main/openapi/samsung-smartthings-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartthings.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: samsungknox.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: developer.smartthings.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api.smartthings.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: docs.samsungknox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Samsung Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Samsung, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Samsung
provider_slug: samsung
slug: samsung-domain-security
source_filename: samsung-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.smartthings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smartthings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\n- host: docs.samsungknox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: smartthings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: samsungknox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samsung/refs/heads/main/security/samsung-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consumer Electronics
- Developer Platform
- IoT
- Mobile
- Smart Home
- Smart TV
- Wearables
---
