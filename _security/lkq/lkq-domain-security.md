---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lkq.com
  spf: true
hosts:
- host: www.lkq.com
  https: false
kind: domain-security
layout: security
method: probed
name: Lkq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LKQ Corporation, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LKQ Corporation
provider_slug: lkq
slug: lkq-domain-security
source_filename: lkq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lkq.com\n  https: false\ndomains:\n- domain: lkq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lkq/refs/heads/main/security/lkq-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Automotive
- Auto Parts
- Fortune 500
- Aftermarket
- Recycled Parts
---
