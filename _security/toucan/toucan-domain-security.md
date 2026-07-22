---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: toucan.earth
  spf: true
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
  domain: thegraph.com
  spf: true
hosts:
- cert_expires: Sep 14 06:45:40 2026 GMT
  host: toucan.earth
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 16:02:01 2026 GMT
  host: docs.toucan.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 04:42:21 2026 GMT
  host: gateway-arbitrum.network.thegraph.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toucan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toucan, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Toucan
provider_slug: toucan
slug: toucan-domain-security
source_filename: toucan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toucan.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:45:40 2026 GMT\n  hsts: false\n- host: docs.toucan.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 16:02:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway-arbitrum.network.thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:42:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: toucan.earth\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thegraph.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toucan/refs/heads/main/security/toucan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Planetary Health
- Carbon Credits
- Climate
- Web3
- Carbon Markets
- Tokenization
- GraphQL
- Biochar
---
