---
api_specs:
- filename: slice-public-api-v1-openapi.yml
  format: yaml
  label: Slice Public API (v1)
  slug: rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slice/refs/heads/main/openapi/slice-public-api-v1-openapi.yml
- filename: slice-public-api-v2-openapi.yml
  format: yaml
  label: Slice Public API (v2)
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slice/refs/heads/main/openapi/slice-public-api-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: slicelife.com
  spf: true
hosts:
- cert_expires: Sep 23 06:33:19 2026 GMT
  host: slicelife.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 14:40:57 2026 GMT
  host: developer.slicelife.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slice, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Slice
provider_slug: slice
slug: slice-domain-security
source_filename: slice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slicelife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:33:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.slicelife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:40:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: slicelife.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slice/refs/heads/main/security/slice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Restaurant
- Pizza
- Online Ordering
- Local Commerce
- Menus
- Orders
---
