---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: b2b.cn
  spf: true
hosts:
- host: corp.b2b.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for corp, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: corp
provider_slug: corp
slug: corp-domain-security
source_filename: corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corp.b2b.cn\n  https: false\ndomains:\n- domain: b2b.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corp/refs/heads/main/security/corp-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
