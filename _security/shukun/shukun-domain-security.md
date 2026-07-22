---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shukun.net
  spf: true
hosts:
- host: shukun.net
  https: false
kind: domain-security
layout: security
method: probed
name: Shukun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shukun, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: shukun
provider_slug: shukun
slug: shukun-domain-security
source_filename: shukun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shukun.net\n  https: false\ndomains:\n- domain: shukun.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shukun/refs/heads/main/security/shukun-domain-security.yml
summary_line: DMARC
tags:
- Company
- Artificial Intelligence
- Healthcare
- Medical Imaging
- Diagnostics
- Machine Learning
- China
---
