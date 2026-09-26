---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: callagent.pro
  spf: true
hosts:
- host: callagent.pro
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Callagentpro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for callagent.pro, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: callagent.pro
provider_slug: callagentpro
slug: callagentpro-domain-security
source_filename: callagentpro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callagent.pro\n  https: false\ndomains:\n- domain: callagent.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callagentpro/refs/heads/main/security/callagentpro-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- AI
- Voice
- Telephony
- Automation
- SaaS
---
