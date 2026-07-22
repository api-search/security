---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infinifi.xyz
  spf: true
hosts:
- cert_expires: Aug 27 18:43:18 2026 GMT
  host: infinifi.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infinifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infinifi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Infinifi
provider_slug: infinifi
slug: infinifi-domain-security
source_filename: infinifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infinifi.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:43:18 2026 GMT\n  hsts: false\ndomains:\n- domain: infinifi.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinifi/refs/heads/main/security/infinifi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defi
- Stablecoin
- Yield
- Ethereum
- Smart Contracts
- Fractional Reserve
- Governance
- Pendle
- Ethena
---
