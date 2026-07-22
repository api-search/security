---
api_specs:
- filename: picker-openapi-original.json
  format: json
  label: Picker API
  slug: picker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picker/refs/heads/main/openapi/picker-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pickerexpress.com
  spf: true
hosts:
- cert_expires: Sep 18 23:50:50 2026 GMT
  host: pickerexpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 00:58:07 2026 GMT
  host: www.pickerexpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 11:48:40 2026 GMT
  host: api.pickerexpress.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Picker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Picker, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Picker
provider_slug: picker
slug: picker-domain-security
source_filename: picker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pickerexpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:50:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.pickerexpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 00:58:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pickerexpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:48:40 2026 GMT\n  hsts: null\ndomains:\n- domain: pickerexpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picker/refs/heads/main/security/picker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Delivery
- Last Mile
- Courier
- E-commerce
- Shipping
- Tracking
- Latin America
- Fleet Management
---
