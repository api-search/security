---
api_specs:
- filename: emerge-public-api-openapi.yml
  format: yaml
  label: Emerge Public API (Shipper API)
  slug: emerge-public-api-shipper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-public-api-openapi.yml
- filename: emerge-carrier-api-openapi.yml
  format: yaml
  label: Emerge Carrier API
  slug: emerge-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-carrier-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emergemarket.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: emergemarket.io
  spf: true
hosts:
- cert_expires: Sep 19 20:29:16 2026 GMT
  host: www.emergemarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 22:31:42 2026 GMT
  host: api-docs.emergemarket.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 22:31:42 2026 GMT
  host: api.emergemarket.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emerge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emerge, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Emerge
provider_slug: emerge
slug: emerge-domain-security
source_filename: emerge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emergemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:29:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.emergemarket.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:31:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.emergemarket.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:31:42 2026 GMT\n  hsts: null\ndomains:\n- domain: emergemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: emergemarket.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/security/emerge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- freight
- logistics
- transportation
- supply-chain
- procurement
- trucking
- freight-marketplace
- transportation-management
- shipping
- rate-benchmarking
- webhooks
- b2b-marketplace
---
