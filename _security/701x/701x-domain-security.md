---
api_specs:
- filename: 701x-api-v1-openapi.json
  format: json
  label: 701x API V1
  slug: 701x-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/701x/refs/heads/main/openapi/701x-api-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 701x.com
  spf: true
hosts:
- cert_expires: Nov 15 00:57:07 2026 GMT
  host: www.701x.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.701x.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 701X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 701x, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 701x
provider_slug: 701x
slug: 701x-domain-security
source_filename: 701x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.701x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 00:57:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.701x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 701x.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/701x/refs/heads/main/security/701x-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- AgTech
- Livestock
- Cattle Management
- Ranch Management
- Animal Health
- IoT
- GPS Tracking
- Traceability
- Beef Production
---
