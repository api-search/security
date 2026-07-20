---
api_specs:
- filename: ledgerx-market-data-asyncapi.yml
  format: yaml
  label: MIAXdx Market Data and Account API
  slug: market-data
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ledgerx/refs/heads/main/asyncapi/ledgerx-market-data-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ledgerx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: miaxdx.com
  spf: true
hosts:
- cert_expires: Oct 12 04:38:51 2026 GMT
  host: app.ledgerx.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 00:31:53 2026 GMT
  host: docs.miaxdx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:38:51 2026 GMT
  host: api.ledgerx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ledgerx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LedgerX (MIAX Derivatives Exchange), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: LedgerX (MIAX Derivatives Exchange)
provider_slug: ledgerx
slug: ledgerx-domain-security
source_filename: ledgerx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.ledgerx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:38:51 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.miaxdx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 00:31:53 2026 GMT\n  hsts: null\n- host: api.ledgerx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:38:51 2026 GMT\n  hsts: null\ndomains:\n- domain: ledgerx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: miaxdx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledgerx/refs/heads/main/security/ledgerx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Financial Services
- Derivatives
- Trading
- Cryptocurrency
- Bitcoin
- Exchange
- Market Data
- WebSockets
- Regulated Markets
---
