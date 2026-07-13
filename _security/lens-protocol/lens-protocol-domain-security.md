---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lens.xyz
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: npmjs.com
  spf: true
hosts:
- cert_expires: Sep 29 10:42:08 2026 GMT
  host: lens.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:35:37 2026 GMT
  host: api.lens.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:32:50 2026 GMT
  host: www.npmjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lens Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lens Protocol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lens Protocol
provider_slug: lens-protocol
slug: lens-protocol-domain-security
source_filename: lens-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lens.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:42:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lens.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:35:37 2026 GMT\n  hsts: false\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:32:50 2026 GMT\n  hsts: null\ndomains:\n- domain: lens.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: npmjs.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lens-protocol/refs/heads/main/security/lens-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Lens Protocol
- Onchain Social
- Web3
- Social Graph
- Polygon
- Lens Chain
- zkEVM
- GraphQL
- Smart Contracts
- Decentralized Identity
---
