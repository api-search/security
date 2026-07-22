---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; sp=reject; rua=mailto:dmarc_reports@loopcrypto.xyz,mailto:mike@loopcrypto.xyz; ruf=mailto:dmarc_reports@loopcrypto.xyz,mailto:mike@loopcrypto.xyz; rf=afrf; pct=100; ri=86400
  dmarc_subdomain_policy: reject
  dnssec: true
  dnssec_ds: 36245 13 1 737EF604740A71957D585EE77AE131395D48BDEB
  domain: loopcrypto.xyz
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:22357071.spf04.hubspotemail.net mx ~all
hosts:
- host: www.loopcrypto.xyz
  hsts: null
  https: null
  note: no A record resolvable
  tls_version: null
- host: api.loopcrypto.xyz
  hsts: null
  https: null
  note: no A record resolvable
  tls_version: null
- host: docs.loopcrypto.xyz
  hsts: null
  https: null
  note: no A record resolvable
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Loop Crypto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loop Crypto, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Loop Crypto
provider_slug: loop-crypto
slug: loop-crypto-domain-security
source_filename: loop-crypto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig against public resolvers (1.1.1.1, 8.8.8.8) and the registrar authoritative nameservers\nnote: >-\n  Loop Crypto is winding down (folding into Lead, service sunset 2026-02-13). As of this\n  probe the apex and subdomain A records no longer resolve on public resolvers, so the live\n  TLS/HSTS posture of the hosts could not be measured. The DNS zone (TXT/SPF/DMARC/DNSSEC)\n  is still published. Absence of A records is recorded as observed, not inferred.\nhosts:\n  - {host: www.loopcrypto.xyz, https: null, tls_version: null, hsts: null, note: no A record resolvable}\n  - {host: api.loopcrypto.xyz, https: null, tls_version: null, hsts: null, note: no A record resolvable}\n  - {host: docs.loopcrypto.xyz, https: null, tls_version: null, hsts: null, note: no A record resolvable}\ndomains:\n  - domain: loopcrypto.xyz\n    dnssec: true\n    dnssec_ds: 36245 13 1 737EF604740A71957D585EE77AE131395D48BDEB\n    caa: []\n    spf: true\n\
  \    spf_record: \"v=spf1 include:_spf.google.com include:22357071.spf04.hubspotemail.net mx ~all\"\n    dmarc: true\n    dmarc_policy: reject\n    dmarc_subdomain_policy: reject\n    dmarc_pct: 100\n    dmarc_record: \"v=DMARC1; p=reject; sp=reject; rua=mailto:dmarc_reports@loopcrypto.xyz,mailto:mike@loopcrypto.xyz; ruf=mailto:dmarc_reports@loopcrypto.xyz,mailto:mike@loopcrypto.xyz; rf=afrf; pct=100; ri=86400\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loop-crypto/refs/heads/main/security/loop-crypto-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Payments
- Cryptocurrency
- Stablecoins
- Web3
- Payment Processing
- Billing
- Solana
- Ethereum
---
