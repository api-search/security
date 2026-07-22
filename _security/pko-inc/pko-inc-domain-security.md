---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pko.xyz
  spf: true
hosts:
- host: pko.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: Pko Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PKO Inc., probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PKO Inc.
provider_slug: pko-inc
slug: pko-inc-domain-security
source_filename: pko-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pko.xyz\n  https: false\ndomains:\n- domain: pko.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pko-inc/refs/heads/main/security/pko-inc-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Venture Capital
- Community
- Technology
- Entertainment
- Web3
- Gaming
- Creator Economy
- Metaverse
---
