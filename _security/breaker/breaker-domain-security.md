---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brkr.jp
  spf: true
hosts:
- host: brkr.jp
  https: false
kind: domain-security
layout: security
method: probed
name: Breaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breaker, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Breaker
provider_slug: breaker
slug: breaker-domain-security
source_filename: breaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brkr.jp\n  https: false\ndomains:\n- domain: brkr.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breaker/refs/heads/main/security/breaker-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
