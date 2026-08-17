---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: prelay.com
  spf: true
hosts:
- host: www.prelay.com
  https: false
kind: domain-security
layout: security
method: probed
name: Prelay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prelay, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Prelay
provider_slug: prelay
slug: prelay-domain-security
source_filename: prelay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prelay.com\n  https: false\ndomains:\n- domain: prelay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prelay/refs/heads/main/security/prelay-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Sales
- Revenue Operations
- Deal Collaboration
- Team Selling
- SaaS
---
