---
api_specs:
- filename: hevn-inc-openapi-original.json
  format: json
  label: HEVN API
  slug: hevn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevn-inc/refs/heads/main/openapi/hevn-inc-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gethevn.com
  spf: false
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: mintlify.app
  spf: false
hosts:
- cert_expires: Oct 16 18:00:07 2026 GMT
  host: gethevn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 04:22:31 2026 GMT
  host: hevninc.mintlify.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 04:22:07 2026 GMT
  host: api.hevn.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hevn Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hevn Inc, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Hevn Inc
provider_slug: hevn-inc
slug: hevn-inc-domain-security
source_filename: hevn-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gethevn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 18:00:07 2026 GMT\n  hsts: false\n- host: hevninc.mintlify.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hevn.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 04:22:07 2026 GMT\n  hsts: null\ndomains:\n- domain: gethevn.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: mintlify.app\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hevn-inc/refs/heads/main/security/hevn-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Banking
- Payments
- Stablecoin
- USDC
- Cross-Border Payments
- Business Accounts
- MCP
- Agents
- API
---
