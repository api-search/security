---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 61.com
  spf: true
hosts:
- host: 61.com
  https: false
kind: domain-security
layout: security
method: probed
name: 61 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 61, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: '61'
provider_slug: '61'
slug: 61-domain-security
source_filename: 61-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 61.com\n  https: false\ndomains:\n- domain: 61.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/61/refs/heads/main/security/61-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
