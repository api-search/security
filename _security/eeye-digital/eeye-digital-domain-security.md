---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eeye.com
  spf: true
hosts:
- host: www.eeye.com
  https: false
kind: domain-security
layout: security
method: probed
name: Eeye Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eEye Digital Security, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: eEye Digital Security
provider_slug: eeye-digital
slug: eeye-digital-domain-security
source_filename: eeye-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eeye.com\n  https: false\ndomains:\n- domain: eeye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eeye-digital/refs/heads/main/security/eeye-digital-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cybersecurity
- Vulnerability Management
- Security
- Acquired
- Historical
---
