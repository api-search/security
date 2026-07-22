---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bgogo.com
  spf: true
hosts:
- host: bgogo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bgogo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bgogo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bgogo
provider_slug: bgogo
slug: bgogo-domain-security
source_filename: bgogo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bgogo.com\n  https: false\ndomains:\n- domain: bgogo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bgogo/refs/heads/main/security/bgogo-domain-security.yml
summary_line: DMARC
tags:
- Company
- Crypto
---
