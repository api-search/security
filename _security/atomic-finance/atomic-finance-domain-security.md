---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atomic.finance
  spf: true
hosts:
- host: atomic.finance
  https: false
kind: domain-security
layout: security
method: probed
name: Atomic Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomic Finance, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atomic Finance
provider_slug: atomic-finance
slug: atomic-finance-domain-security
source_filename: atomic-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomic.finance\n  https: false\ndomains:\n- domain: atomic.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomic-finance/refs/heads/main/security/atomic-finance-domain-security.yml
summary_line: DMARC
tags:
- Company
- Crypto
- Bitcoin
- Discreet Log Contracts
- DLC
- Non-Custodial
- Options Trading
- Open Source
- Lightning Network
---
