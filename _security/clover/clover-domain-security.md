---
api_specs:
- filename: clover-platform-rest-api-openapi.yml
  format: yaml
  label: Clover REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-platform-rest-api-openapi.yml
- filename: clover-ecommerce-api-openapi.yml
  format: yaml
  label: Clover Ecommerce API
  slug: ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/openapi/clover-ecommerce-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clover.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.clover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 26 12:47:22 2026 GMT
  host: docs.clover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.clover.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clover, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clover
provider_slug: clover
slug: clover-domain-security
source_filename: clover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clover.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.clover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 12:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clover.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: clover.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/security/clover-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Restaurant
- POS
- Payments
- Retail
- SMB
- Hardware
---
