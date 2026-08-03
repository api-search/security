---
api_specs:
- filename: leaflink-api-openapi-original.yml
  format: yaml
  label: LeafLink API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/openapi/leaflink-api-openapi-original.yml
- filename: leaflink-marketplace-v2-openapi-original.yml
  format: yaml
  label: LeafLink Marketplace V2 API
  slug: marketplace-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/openapi/leaflink-marketplace-v2-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leaflink.com
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.leaflink.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: staging-api.leaflink.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leaflink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeafLink, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LeafLink
provider_slug: leaflink
slug: leaflink-domain-security
source_filename: leaflink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: api.leaflink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: staging-api.leaflink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: leaflink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaflink/refs/heads/main/security/leaflink-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cannabis
- Wholesale
- B2B Marketplace
- Supply Chain
- Payments
- Logistics
- Inventory
- Compliance
- Traceability
- eCommerce
- Distribution
- Retail
---
