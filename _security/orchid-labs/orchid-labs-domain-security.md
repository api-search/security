---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: orchid.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.orchid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orchid Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orchid Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Orchid Labs
provider_slug: orchid-labs
slug: orchid-labs-domain-security
source_filename: orchid-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orchid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orchid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orchid-labs/refs/heads/main/security/orchid-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- VPN
- Privacy
- Decentralized
- Blockchain
- Cryptocurrency
- Nanopayments
- Web3
- Networking
---
