---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cmlabs.com.cn
  spf: true
hosts:
- host: cmlabs.com.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Cmlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cmlabs, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: cmlabs
provider_slug: cmlabs
slug: cmlabs-domain-security
source_filename: cmlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cmlabs.com.cn\n  https: false\ndomains:\n- domain: cmlabs.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cmlabs/refs/heads/main/security/cmlabs-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Healthcare
- Clinical Laboratory
- Diagnostics
- Medical Testing
- Life Sciences
- China
---
