---
api_specs:
- filename: fulcrumpro-openapi-original.json
  format: json
  label: Fulcrum Public API
  slug: fulcrum-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulcrumpro/refs/heads/main/openapi/fulcrumpro-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fulcrumpro.com
  spf: true
hosts:
- cert_expires: Sep 22 01:31:40 2026 GMT
  host: api.fulcrumpro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fulcrumpro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fulcrumpro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Fulcrumpro
provider_slug: fulcrumpro
slug: fulcrumpro-domain-security
source_filename: fulcrumpro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.fulcrumpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:31:40 2026 GMT\n  hsts: null\ndomains:\n- domain: fulcrumpro.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulcrumpro/refs/heads/main/security/fulcrumpro-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Manufacturing
- ERP
- MES
- Manufacturing Execution
- Job Shop
- CNC Machining
- Sheet Metal
- Inventory
- Purchasing
- Quoting
- Scheduling
---
