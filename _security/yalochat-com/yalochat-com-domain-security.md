---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yalochat.com
  spf: true
hosts:
- host: yalochat.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yalochat Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yalo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yalo
provider_slug: yalochat-com
slug: yalochat-com-domain-security
source_filename: yalochat-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yalochat.com\n  https: false\ndomains:\n- domain: yalochat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/yalochat-com/security/yalochat-com-domain-security.yml
summary_line: DMARC
tags:
- AI
- Conversational
- Sales
- CustomerEngagement
- WhatsApp
---
