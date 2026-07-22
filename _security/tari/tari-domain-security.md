---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tari.com
  spf: true
hosts:
- cert_expires: Oct 16 13:52:38 2026 GMT
  host: tari.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tari, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tari
provider_slug: tari
slug: tari-domain-security
source_filename: tari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 13:52:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: tari.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tari/refs/heads/main/security/tari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Cryptocurrency
- Protocol
- gRPC
- Wallet
- Mining
- Privacy
- Web3
---
