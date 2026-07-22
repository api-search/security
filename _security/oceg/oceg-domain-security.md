---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oceg.com
  spf: true
hosts:
- host: oceg.com
  https: false
kind: domain-security
layout: security
method: probed
name: Oceg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for oceg, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: oceg
provider_slug: oceg
slug: oceg-domain-security
source_filename: oceg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oceg.com\n  https: false\ndomains:\n- domain: oceg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oceg/refs/heads/main/security/oceg-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
