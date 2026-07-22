---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: neuroware.io
  spf: true
hosts:
- cert_expires: Aug 30 16:41:16 2026 GMT
  host: neuroware.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neurowareio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neuroware.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Neuroware.io
provider_slug: neurowareio
slug: neurowareio-domain-security
source_filename: neurowareio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neuroware.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 16:41:16 2026 GMT\n  hsts: false\ndomains:\n- domain: neuroware.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurowareio/refs/heads/main/security/neurowareio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Blockchain
- Distributed Ledger
- Cryptocurrency
- Digital Asset Custody
- Wallet Infrastructure
- Fintech
- Web3
---
