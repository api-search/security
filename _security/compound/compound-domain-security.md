---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: compound.finance
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thegraph.com
  spf: true
hosts:
- cert_expires: Oct  8 21:46:51 2026 GMT
  host: compound.finance
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:49:39 2026 GMT
  host: api.thegraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Compound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compound Finance, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Compound Finance
provider_slug: compound
slug: compound-domain-security
source_filename: compound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compound.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:46:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:49:39 2026 GMT\n  hsts: null\ndomains:\n- domain: compound.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thegraph.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compound/refs/heads/main/security/compound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Lending
- Borrowing
- Ethereum
- Blockchain
- Finance
- Cryptocurrency
---
