---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wecook.cn
  spf: true
hosts:
- host: www.wecook.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Wecook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeCook, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WeCook
provider_slug: wecook
slug: wecook-domain-security
source_filename: wecook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wecook.cn\n  https: false\ndomains:\n- domain: wecook.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wecook/refs/heads/main/security/wecook-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
---
