---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: towns.com
  spf: true
hosts:
- cert_expires: Sep  1 11:02:45 2026 GMT
  host: www.towns.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 04:48:31 2026 GMT
  host: docs.towns.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:12:05 2026 GMT
  host: app.towns.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Here Not There Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Here Not There Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Here Not There Labs
provider_slug: here-not-there-labs
slug: here-not-there-labs-domain-security
source_filename: here-not-there-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.towns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:02:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.towns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:48:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.towns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:12:05 2026 GMT\n  hsts: false\ndomains:\n- domain: towns.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/here-not-there-labs/refs/heads/main/security/here-not-there-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Messaging
- Decentralized
- Web3
- Blockchain
- Protocol
- Chat
- Bots
- Encryption
- SDK
---
