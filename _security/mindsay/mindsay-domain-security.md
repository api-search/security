---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mindsay.com
  spf: false
hosts:
- host: www.mindsay.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mindsay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mindsay, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Mindsay
provider_slug: mindsay
slug: mindsay-domain-security
source_filename: mindsay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mindsay.com\n  https: false\ndomains:\n- domain: mindsay.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindsay/refs/heads/main/security/mindsay-domain-security.yml
summary_line: DMARC
tags:
- Company
- Ai/Ml
- Conversational AI
- Chatbots
- Customer Service
- Automation
---
