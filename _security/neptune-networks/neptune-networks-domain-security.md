---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: realqmarkets.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: neptunefi.com
  spf: true
hosts:
- cert_expires: Dec 19 07:21:21 2026 GMT
  host: realqmarkets.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 17:25:43 2026 GMT
  host: neptunefi.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neptune Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neptune Networks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neptune Networks
provider_slug: neptune-networks
slug: neptune-networks-domain-security
source_filename: neptune-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: realqmarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 07:21:21 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: neptunefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:25:43 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: realqmarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: neptunefi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neptune-networks/refs/heads/main/security/neptune-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fixed Income
- Capital Markets
- Fintech
- Market Data
- Pre-Trade
- Bonds
- Liquidity
---
