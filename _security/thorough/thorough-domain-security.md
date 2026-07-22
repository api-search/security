---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thorough.ai
  spf: true
hosts:
- host: thorough.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Thorough Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for thorough, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: thorough
provider_slug: thorough
slug: thorough-domain-security
source_filename: thorough-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thorough.ai\n  https: false\ndomains:\n- domain: thorough.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thorough/refs/heads/main/security/thorough-domain-security.yml
summary_line: DMARC
tags:
- Company
- China
- Startup
- Qiming
- Venture Backed
---
