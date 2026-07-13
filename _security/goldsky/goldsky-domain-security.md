---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goldsky.com
  spf: true
hosts:
- cert_expires: Oct  6 16:32:58 2026 GMT
  host: goldsky.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 06:28:29 2026 GMT
  host: docs.goldsky.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:00:47 2026 GMT
  host: api.goldsky.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goldsky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goldsky, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Goldsky
provider_slug: goldsky
slug: goldsky-domain-security
source_filename: goldsky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goldsky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:32:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.goldsky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:28:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.goldsky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:00:47 2026 GMT\n  hsts: null\ndomains:\n- domain: goldsky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goldsky/refs/heads/main/security/goldsky-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain Data
- Indexer
- Subgraphs
- CDC
- Streaming
- RPC
- Crypto
- Web3
---
