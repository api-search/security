---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cutt.com
  spf: true
hosts:
- host: cutt.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cutt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cutt, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: cutt
provider_slug: cutt
slug: cutt-domain-security
source_filename: cutt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cutt.com\n  https: false\ndomains:\n- domain: cutt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cutt/refs/heads/main/security/cutt-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Venture Backed
- Qiming Portfolio
- China
- Portfolio Lead
- Unverified API Surface
- Dormant
---
