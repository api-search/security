---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitbond.com
  spf: true
hosts:
- cert_expires: Sep 19 00:45:24 2026 GMT
  host: www.bitbond.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 08:44:44 2026 GMT
  host: docs.bitbond.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 00:45:24 2026 GMT
  host: om.bitbond.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitbond Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitbond, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bitbond
provider_slug: bitbond
slug: bitbond-domain-security
source_filename: bitbond-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitbond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 00:45:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bitbond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 08:44:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: om.bitbond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 00:45:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bitbond.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitbond/refs/heads/main/security/bitbond-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tokenization
- Blockchain
- Digital Assets
- Smart Contracts
- Web3
- Securities
- Payments
- MCP
---
