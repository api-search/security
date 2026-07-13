---
api_specs:
- filename: bluecart-openapi.yml
  format: yaml
  label: BlueCart API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecart/refs/heads/main/openapi/bluecart-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bluecart.com
  spf: true
hosts:
- cert_expires: Sep 29 03:37:21 2026 GMT
  host: www.bluecart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:13:20 2026 GMT
  host: docs.bluecart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluecart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlueCart, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BlueCart
provider_slug: bluecart
slug: bluecart-domain-security
source_filename: bluecart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bluecart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:37:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.bluecart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:13:20 2026 GMT\n  hsts: false\ndomains:\n- domain: bluecart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecart/refs/heads/main/security/bluecart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Procurement
- Wholesale
- Ordering
- Food Distribution
- Hospitality
- eCommerce
---
