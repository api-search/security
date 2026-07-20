---
api_specs:
- filename: brale-openapi-original.yml
  format: yaml
  label: Brale Issuance and Orchestration API
  slug: brale-issuance-and-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brale/refs/heads/main/openapi/brale-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: brale.xyz
  spf: true
hosts:
- cert_expires: Sep 17 02:28:21 2026 GMT
  host: docs.brale.xyz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 04:52:00 2026 GMT
  host: api.brale.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brale, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Brale
provider_slug: brale
slug: brale-domain-security
source_filename: brale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.brale.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.brale.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:52:00 2026 GMT\n  hsts: null\ndomains:\n- domain: brale.xyz\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brale/refs/heads/main/security/brale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Stablecoins
- Stablecoin Issuance
- Payments
- Blockchain
- Cryptocurrency
- Fintech
- Financial Services
- Custody
- Tokenization
- On-Ramp
- Off-Ramp
---
