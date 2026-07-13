---
api_specs:
- filename: amplifier-gmp-api.yaml
  format: yaml
  label: Axelar Amplifier GMP API
  slug: amplifier-gmp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axelar/refs/heads/main/openapi/amplifier-gmp-api.yaml
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
  dmarc_policy: reject
  dnssec: true
  domain: axelar.network
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: axelarscan.io
  spf: true
hosts:
- cert_expires: Sep 30 17:50:21 2026 GMT
  host: axelar.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 09:28:46 2026 GMT
  host: docs.axelarscan.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:39 2026 GMT
  host: api.axelarscan.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axelar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axelar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Axelar
provider_slug: axelar
slug: axelar-domain-security
source_filename: axelar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axelar.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:50:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.axelarscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:28:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.axelarscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:39 2026 GMT\n  hsts: null\ndomains:\n- domain: axelar.network\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: axelarscan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axelar/refs/heads/main/security/axelar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cross-Chain
- Interoperability
- Web3
- General Message Passing
- Token Bridge
- Cosmos
- EVM
---
