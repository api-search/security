---
api_specs:
- filename: omniful-inc-openapi.yml
  format: yaml
  label: Omniful Integration APIs
  slug: omniful-integration-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omniful-inc/refs/heads/main/openapi/omniful-inc-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: omniful.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: omniful.tech
  spf: false
hosts:
- cert_expires: Sep 29 20:04:09 2026 GMT
  host: www.omniful.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 09:15:02 2026 GMT
  host: docs.omniful.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 05:03:53 2026 GMT
  host: prodapi.omniful.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omniful Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omniful, Inc., probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Omniful, Inc.
provider_slug: omniful-inc
slug: omniful-inc-domain-security
source_filename: omniful-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omniful.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:04:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.omniful.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 09:15:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prodapi.omniful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:03:53 2026 GMT\n  hsts: null\ndomains:\n- domain: omniful.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: omniful.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omniful-inc/refs/heads/main/security/omniful-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Supply Chain
- Fulfillment
- Order Management
- Warehouse Management
- Transportation Management
- Inventory
- Returns
- E-commerce
- Logistics
---
