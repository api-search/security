---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frontis.cn
  spf: true
hosts:
- host: frontis.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Frontis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for frontis, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: frontis
provider_slug: frontis
slug: frontis-domain-security
source_filename: frontis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frontis.cn\n  https: false\ndomains:\n- domain: frontis.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontis/refs/heads/main/security/frontis-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
