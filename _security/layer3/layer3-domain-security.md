---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: layer3.xyz
  spf: true
hosts:
- cert_expires: Oct 17 20:05:29 2026 GMT
  host: layer3.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Layer3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Layer3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Layer3
provider_slug: layer3
slug: layer3-domain-security
source_filename: layer3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layer3.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 20:05:29 2026 GMT\n  hsts: false\ndomains:\n- domain: layer3.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layer3/refs/heads/main/security/layer3-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Web3
- Blockchain
- DeFi
- Rewards
- Onboarding
- Wallet
- Quests
---
