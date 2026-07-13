---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thegraph.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: streamingfast.io
  spf: true
hosts:
- cert_expires: Oct  6 21:32:21 2026 GMT
  host: thegraph.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 11:56:58 2026 GMT
  host: token-api.thegraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 19:34:26 2026 GMT
  host: mainnet.eth.streamingfast.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Graph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Graph, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: The Graph
provider_slug: the-graph
slug: the-graph-domain-security
source_filename: the-graph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:32:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: token-api.thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:56:58 2026 GMT\n  hsts: null\n- host: mainnet.eth.streamingfast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:34:26 2026 GMT\n  hsts: false\ndomains:\n- domain: thegraph.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: streamingfast.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-graph/refs/heads/main/security/the-graph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Indexing
- GraphQL
- Subgraphs
- Multi-chain
---
