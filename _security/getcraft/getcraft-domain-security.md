---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getcraft.com
  spf: true
hosts:
- host: marketingcraft.getcraft.com
  https: false
kind: domain-security
layout: security
method: probed
name: Getcraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetCraft, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GetCraft
provider_slug: getcraft
slug: getcraft-domain-security
source_filename: getcraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketingcraft.getcraft.com\n  https: false\ndomains:\n- domain: getcraft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getcraft/refs/heads/main/security/getcraft-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Content Marketing
- Creative Marketplace
- Freelance Talent
- Advertising
- Marketing
- Indonesia
- Southeast Asia
---
