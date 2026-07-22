---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geode.fi
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: geode.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Geode
provider_slug: geode
slug: geode-domain-security
source_filename: geode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geode.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: geode.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geode/refs/heads/main/security/geode-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- DeFi
- Liquid Staking
- Ethereum
- Avalanche
- Staking
- Blockchain
- Node Operators
---
