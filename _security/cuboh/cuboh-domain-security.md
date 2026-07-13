---
api_specs:
- filename: cuboh-openapi.yml
  format: yaml
  label: Cuboh Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-openapi.yml
- filename: cuboh-openapi.yml
  format: yaml
  label: Cuboh Menu API
  slug: menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-openapi.yml
- filename: cuboh-openapi.yml
  format: yaml
  label: Cuboh Merchant Locations API
  slug: locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-openapi.yml
- filename: cuboh-openapi.yml
  format: yaml
  label: Cuboh Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/openapi/cuboh-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cuboh.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cuboh.net
  spf: false
hosts:
- cert_expires: Sep 10 04:47:51 2026 GMT
  host: www.cuboh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: docs.cuboh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: core.cuboh.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cuboh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuboh, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cuboh
provider_slug: cuboh
slug: cuboh-domain-security
source_filename: cuboh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cuboh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:47:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cuboh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: core.cuboh.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cuboh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cuboh.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/security/cuboh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Online Ordering
- Delivery
- POS
- Order Aggregation
---
