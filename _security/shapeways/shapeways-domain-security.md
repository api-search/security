---
api_specs:
- filename: shapeways-openapi.yml
  format: yaml
  label: Shapeways API
  slug: shapeways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapeways/refs/heads/main/openapi/shapeways-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shapeways.com
  spf: true
hosts:
- cert_expires: Aug 26 11:00:43 2026 GMT
  host: shapeways.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shapeways Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shapeways, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shapeways
provider_slug: shapeways
slug: shapeways-domain-security
source_filename: shapeways-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shapeways.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 11:00:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shapeways.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapeways/refs/heads/main/security/shapeways-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- 3D Printing
- Additive Manufacturing
- Manufacturing
- Prototyping
- Hardware
- Fulfillment
- eCommerce
---
