---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: webb.tools
  spf: true
hosts:
- host: webb.tools
  https: false
kind: domain-security
layout: security
method: probed
name: Webb Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webb Protocol, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Webb Protocol
provider_slug: webb-protocol
slug: webb-protocol-domain-security
source_filename: webb-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: webb.tools\n  https: false\ndomains:\n- domain: webb.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webb-protocol/refs/heads/main/security/webb-protocol-domain-security.yml
summary_line: DMARC
tags:
- Company
- Privacy
---
