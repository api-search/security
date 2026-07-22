---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zhixiaole.com
  spf: true
hosts:
- host: zhixiaole.com
  https: false
kind: domain-security
layout: security
method: probed
name: Zhixiaole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zhixiaole, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: zhixiaole
provider_slug: zhixiaole
slug: zhixiaole-domain-security
source_filename: zhixiaole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zhixiaole.com\n  https: false\ndomains:\n- domain: zhixiaole.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zhixiaole/refs/heads/main/security/zhixiaole-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
