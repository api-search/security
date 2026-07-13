---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coindesk.com
  spf: true
hosts:
- host: old.coindesk.com
  https: false
kind: domain-security
layout: security
method: probed
name: Coindesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinDesk, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoinDesk
provider_slug: coindesk
slug: coindesk-domain-security
source_filename: coindesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: old.coindesk.com\n  https: false\ndomains:\n- domain: coindesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coindesk/refs/heads/main/security/coindesk-domain-security.yml
summary_line: DMARC
tags:
- Cryptocurrency
- Public APIs
---
