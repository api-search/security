---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryroll.com
  spf: true
hosts:
- host: tryroll.com
  https: false
kind: domain-security
layout: security
method: probed
name: Roll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roll, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Roll
provider_slug: roll
slug: roll-domain-security
source_filename: roll-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryroll.com\n  https: false\ndomains:\n- domain: tryroll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roll/refs/heads/main/security/roll-domain-security.yml
summary_line: DMARC
tags:
- Company
- Social Tokens
- Creator Economy
- Blockchain
- Ethereum
- Web3
- Defunct
---
