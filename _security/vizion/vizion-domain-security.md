---
api_specs:
- filename: vizion-container-tracking-openapi.yml
  format: yaml
  label: Vizion Container Tracking API
  slug: container-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vizion/refs/heads/main/openapi/vizion-container-tracking-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vizionapi.com
  spf: true
hosts:
- cert_expires: Aug 16 10:47:43 2026 GMT
  host: www.vizionapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 14:43:51 2026 GMT
  host: docs.vizionapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: prod.vizionapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vizion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vizion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vizion
provider_slug: vizion
slug: vizion-domain-security
source_filename: vizion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vizionapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 10:47:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.vizionapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:43:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod.vizionapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vizionapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vizion/refs/heads/main/security/vizion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Container Tracking
- Logistics
- Ocean Freight
- Shipping
- Supply Chain
- Webhooks
---
