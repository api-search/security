---
api_specs:
- filename: crossmint-openapi.yml
  format: yaml
  label: Crossmint Wallets API
  slug: wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crossmint.com
  spf: true
hosts:
- cert_expires: Aug 25 20:31:32 2026 GMT
  host: www.crossmint.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 04:50:36 2026 GMT
  host: docs.crossmint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 03:45:02 2026 GMT
  host: staging.crossmint.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crossmint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossmint, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crossmint
provider_slug: crossmint
slug: crossmint-domain-security
source_filename: crossmint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossmint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 20:31:32 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.crossmint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:50:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: staging.crossmint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 03:45:02 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: crossmint.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/security/crossmint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Wallets
- NFT
- Payments
- Checkout
---
