---
api_specs:
- filename: openapi
  format: yaml
  label: ConvertAPI
  slug: convertapi
  spec_type: OpenAPI
  url: https://v2.convertapi.com/info/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: convertapi.com
  spf: true
hosts:
- cert_expires: Sep  3 16:02:21 2026 GMT
  host: www.convertapi.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: v2.convertapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: eu-v2.convertapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convertapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConvertAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ConvertAPI
provider_slug: convertapi
slug: convertapi-domain-security
source_filename: convertapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.convertapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: v2.convertapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\n- host: eu-v2.convertapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: convertapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertapi/refs/heads/main/security/convertapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Conversion
- PDF
- Documents
- Images
- Audio
- Video
- E-books
- Office Documents
- Batch Processing
---
