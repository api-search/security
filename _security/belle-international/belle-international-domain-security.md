---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: belle.com.cn
  spf: true
hosts:
- host: www.belle.com.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Belle International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belle International, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Belle International
provider_slug: belle-international
slug: belle-international-domain-security
source_filename: belle-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.belle.com.cn\n  https: false\ndomains:\n- domain: belle.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belle-international/refs/heads/main/security/belle-international-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Retail
- Footwear
- Fashion
- Apparel
- E-Commerce
- Consumer
- China
---
