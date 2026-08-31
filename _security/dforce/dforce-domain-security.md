---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dforce.network
  spf: true
hosts:
- cert_expires: Aug 21 14:57:17 2026 GMT
  host: dforce.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dforce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dForce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: dForce
provider_slug: dforce
slug: dforce-domain-security
source_filename: dforce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dforce.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 14:57:17 2026 GMT\n  hsts: false\ndomains:\n- domain: dforce.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dforce/refs/heads/main/security/dforce-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- DeFi
- Stablecoin
- Lending
- Blockchain
- RWA
- Bridge
- Governance
---
