---
api_specs:
- filename: oto-global-openapi.yml
  format: yaml
  label: OTO API V2
  slug: oto-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oto-global/refs/heads/main/openapi/oto-global-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tryoto.com
  spf: true
hosts:
- cert_expires: Sep  4 12:54:12 2026 GMT
  host: tryoto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 17:33:00 2026 GMT
  host: apis.tryoto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 11:25:53 2026 GMT
  host: api.tryoto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oto Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OTO Global, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OTO Global
provider_slug: oto-global
slug: oto-global-domain-security
source_filename: oto-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryoto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 12:54:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apis.tryoto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:33:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tryoto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 11:25:53 2026 GMT\n  hsts: null\ndomains:\n- domain: tryoto.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oto-global/refs/heads/main/security/oto-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Shipping
- Logistics
- Fulfillment
- E-commerce
- Delivery
- Carriers
- Returns
- Saudi Arabia
---
