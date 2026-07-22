---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: knote.com
  spf: true
hosts:
- host: knote.com
  https: false
kind: domain-security
layout: security
method: probed
name: Knote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knote, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Knote
provider_slug: knote
slug: knote-domain-security
source_filename: knote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knote.com\n  https: false\ndomains:\n- domain: knote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knote/refs/heads/main/security/knote-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Startup
- Knowledge Management
- Notes
- Productivity
- Collaboration
- 500 Global
- Dormant
---
