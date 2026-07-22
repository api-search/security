---
api_specs:
- filename: uniuni-platform-client-api-openapi.yml
  format: yaml
  label: UniUni Platform Client API
  slug: uniuni-platform-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniuni/refs/heads/main/openapi/uniuni-platform-client-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uniuni.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.uniuni.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 10:12:32 2026 GMT
  host: help.ship.uniuni.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.ship.uniuni.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uniuni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UniUni, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UniUni
provider_slug: uniuni
slug: uniuni-domain-security
source_filename: uniuni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uniuni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\n- host: help.ship.uniuni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:12:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ship.uniuni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: uniuni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniuni/refs/heads/main/security/uniuni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Shipping
- Last-Mile Delivery
- Ecommerce
- Tracking
- Delivery
---
