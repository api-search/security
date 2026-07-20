---
api_specs:
- filename: due-openapi-original.yml
  format: yaml
  label: Due API
  slug: due-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/openapi/due-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: due.network
  spf: true
hosts:
- cert_expires: Aug 23 23:59:59 2026 GMT
  host: api.due.network
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 11:38:15 2026 GMT
  host: api.sandbox.due.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Due Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Due, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Due
provider_slug: due
slug: due-domain-security
source_filename: due-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.due.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:59:59 2026 GMT\n  hsts: null\n- host: api.sandbox.due.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:38:15 2026 GMT\n  hsts: null\ndomains:\n- domain: due.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/due/refs/heads/main/security/due-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Cross-Border Payments
- Stablecoins
- Fintech
- Virtual Accounts
- Foreign Exchange
- KYC
- Wallets
- API
---
