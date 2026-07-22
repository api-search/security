---
api_specs:
- filename: obol-openapi-original.json
  format: json
  label: Obol API
  slug: obol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-openapi-original.json
- filename: docs-json
  format: yaml
  label: Obol API OpenAPI (live)
  slug: obol-api-openapi-live
  spec_type: OpenAPI
  url: https://api.obol.tech/docs-json
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: obol.tech
  spf: true
hosts:
- cert_expires: Sep 29 00:14:31 2026 GMT
  host: obol.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Obol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Obol
provider_slug: obol
slug: obol-domain-security
source_filename: obol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obol.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:14:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: obol.tech\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/security/obol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Ethereum
- Staking
- Distributed Validators
- Blockchain Infrastructure
- Web3
---
