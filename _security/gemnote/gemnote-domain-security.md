---
api_specs:
- filename: gemnote-openapi.yml
  format: yaml
  label: Gemnote API
  slug: gemnote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemnote/refs/heads/main/openapi/gemnote-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gemnote.com
  spf: true
hosts:
- cert_expires: Sep 11 19:45:07 2026 GMT
  host: www.gemnote.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 00:04:24 2026 GMT
  host: api.gemnote.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 01:51:29 2026 GMT
  host: sandbox.gemnote.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gemnote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gemnote, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gemnote
provider_slug: gemnote
slug: gemnote-domain-security
source_filename: gemnote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gemnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:45:07 2026 GMT\n  hsts: false\n- host: api.gemnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandbox.gemnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 01:51:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gemnote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemnote/refs/heads/main/security/gemnote-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Corporate Gifting
- Swag Management
- Branded Merchandise
- Fulfillment
- E-commerce
- Shipping
- Y Combinator
---
