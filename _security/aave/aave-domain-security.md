---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aave.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thegraph.com
  spf: true
hosts:
- cert_expires: Oct  3 02:45:11 2026 GMT
  host: aave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:49:39 2026 GMT
  host: api.thegraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:28:04 2026 GMT
  host: app.aave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aave, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aave
provider_slug: aave
slug: aave-domain-security
source_filename: aave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:45:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:49:39 2026 GMT\n  hsts: null\n- host: app.aave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:28:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aave.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thegraph.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aave/refs/heads/main/security/aave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Lending
- Borrowing
- Liquidity
- Protocol
- Subgraph
- GraphQL
---
