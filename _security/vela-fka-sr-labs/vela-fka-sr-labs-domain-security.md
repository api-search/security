---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tradevela.com
  spf: true
hosts:
- host: tradevela.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vela Fka Sr Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vela (FKA SR Labs), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vela (FKA SR Labs)
provider_slug: vela-fka-sr-labs
slug: vela-fka-sr-labs-domain-security
source_filename: vela-fka-sr-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradevela.com\n  https: false\ndomains:\n- domain: tradevela.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vela-fka-sr-labs/refs/heads/main/security/vela-fka-sr-labs-domain-security.yml
summary_line: DMARC
tags:
- Company
- Financial
- Market Data
- Trading
- Low Latency
- Options
- OpenMAMA
- Defunct
---
