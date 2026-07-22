---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oriongeo.com
  spf: true
hosts:
- host: oriongeo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ripa Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RIPA AI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RIPA AI
provider_slug: ripa-ai
slug: ripa-ai-domain-security
source_filename: ripa-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oriongeo.com\n  https: false\ndomains:\n- domain: oriongeo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripa-ai/refs/heads/main/security/ripa-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
---
