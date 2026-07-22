---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chatail.com
  spf: true
hosts:
- host: chatail.com
  https: false
kind: domain-security
layout: security
method: probed
name: Chatail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for chatail, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: chatail
provider_slug: chatail
slug: chatail-domain-security
source_filename: chatail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chatail.com\n  https: false\ndomains:\n- domain: chatail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatail/refs/heads/main/security/chatail-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- SaaS
- Live Commerce
- Video
- Retail
- Customer Engagement
- China
---
