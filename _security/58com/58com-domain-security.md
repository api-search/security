---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 58.com
  spf: true
hosts:
- host: bj.58.com
  https: false
kind: domain-security
layout: security
method: probed
name: 58Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 58.com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 58.com
provider_slug: 58com
slug: 58com-domain-security
source_filename: 58com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bj.58.com\n  https: false\ndomains:\n- domain: 58.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/58com/refs/heads/main/security/58com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- Classifieds
- Marketplace
- Real Estate
- Recruitment
- Local Services
- China
---
