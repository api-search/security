---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zd-med.com
  spf: true
hosts:
- host: zd-med.com
  https: false
kind: domain-security
layout: security
method: probed
name: Zd Med Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zd-med, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: zd-med
provider_slug: zd-med
slug: zd-med-domain-security
source_filename: zd-med-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zd-med.com\n  https: false\ndomains:\n- domain: zd-med.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zd-med/refs/heads/main/security/zd-med-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
