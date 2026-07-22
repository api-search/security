---
description: ''
domains:
- caa:
  - haoyiku.com.cn.w.kunlunpi.com.
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haoyiku.com.cn
  spf: true
hosts:
- host: haoyiku.com.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Haoyiku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for haoyiku, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: haoyiku
provider_slug: haoyiku
slug: haoyiku-domain-security
source_filename: haoyiku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haoyiku.com.cn\n  https: false\ndomains:\n- domain: haoyiku.com.cn\n  dnssec: false\n  caa:\n  - haoyiku.com.cn.w.kunlunpi.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haoyiku/refs/heads/main/security/haoyiku-domain-security.yml
summary_line: DMARC
tags:
- Company
- E-Commerce
- Social Commerce
- Retail
- Mobile Apps
- China
- Consumer
---
