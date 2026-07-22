---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qiangsenmedical.com
  spf: true
hosts:
- host: qiangsenmedical.com
  https: false
kind: domain-security
layout: security
method: probed
name: Qiangsenmedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for qiangsenmedical, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: qiangsenmedical
provider_slug: qiangsenmedical
slug: qiangsenmedical-domain-security
source_filename: qiangsenmedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qiangsenmedical.com\n  https: false\ndomains:\n- domain: qiangsenmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qiangsenmedical/refs/heads/main/security/qiangsenmedical-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
