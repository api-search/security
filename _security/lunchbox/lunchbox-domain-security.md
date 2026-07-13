---
api_specs:
- filename: lunchbox-core-openapi.yml
  format: yaml
  label: Lunchbox Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/openapi/lunchbox-core-openapi.yml
- filename: lunchbox-management-openapi.yml
  format: yaml
  label: Lunchbox Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/openapi/lunchbox-management-openapi.yml
- filename: lunchbox-loyalty-openapi.yml
  format: yaml
  label: Lunchbox Loyalty API
  slug: loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/openapi/lunchbox-loyalty-openapi.yml
- filename: lunchbox-pos-openapi.yml
  format: yaml
  label: Lunchbox POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/openapi/lunchbox-pos-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lunchbox.io
  spf: true
hosts:
- cert_expires: Aug 29 10:41:45 2026 GMT
  host: lunchbox.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 13:55:08 2026 GMT
  host: docs.lunchbox.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lunchbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunchbox, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lunchbox
provider_slug: lunchbox
slug: lunchbox-domain-security
source_filename: lunchbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lunchbox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 10:41:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lunchbox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:55:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lunchbox.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunchbox/refs/heads/main/security/lunchbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Online Ordering
- Guest Engagement
- Catering
- Menus
- Orders
- Loyalty
- Enterprise
---
