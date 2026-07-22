---
api_specs:
- filename: symbiotic-relay-openapi.json
  format: json
  label: Symbiotic Relay API
  slug: symbiotic-relay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symbiotic/refs/heads/main/openapi/symbiotic-relay-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: symbiotic.fi
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: symbiotic.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Symbiotic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symbiotic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Symbiotic
provider_slug: symbiotic
slug: symbiotic-domain-security
source_filename: symbiotic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: symbiotic.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: symbiotic.fi\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symbiotic/refs/heads/main/security/symbiotic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Defi
- Restaking
- Shared Security
- Staking
- Blockchain
- Web3
- Smart Contracts
- Ethereum
- DeFi
---
