---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: faraway.com
  spf: true
hosts:
- cert_expires: Sep 21 15:58:53 2026 GMT
  host: faraway.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:28:10 2026 GMT
  host: docs.faraway.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 15:58:53 2026 GMT
  host: api.faraway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Faraway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faraway, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Faraway
provider_slug: faraway
slug: faraway-domain-security
source_filename: faraway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faraway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:58:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.faraway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:28:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.faraway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:58:53 2026 GMT\n  hsts: null\ndomains:\n- domain: faraway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faraway/refs/heads/main/security/faraway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Web3
- Blockchain
- Gaming Economy
- Player Identity
- Marketplace
- Creator Platform
- NFT
- Developer Platform
---
