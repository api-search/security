---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: longwill.com.cn
  spf: true
hosts:
- host: longwill.com.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Longwill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for longwill, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: longwill
provider_slug: longwill
slug: longwill-domain-security
source_filename: longwill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: longwill.com.cn\n  https: false\ndomains:\n- domain: longwill.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/longwill/refs/heads/main/security/longwill-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Health
- Elder Care
- Community Health
- Digital Health
- China
- Qiming Portfolio
---
