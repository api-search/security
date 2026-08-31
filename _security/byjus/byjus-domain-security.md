---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: byjus.com
  spf: true
hosts:
- host: byjus.com
  https: false
kind: domain-security
layout: security
method: probed
name: Byjus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Byjus, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Byjus
provider_slug: byjus
slug: byjus-domain-security
source_filename: byjus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: byjus.com\n  https: false\ndomains:\n- domain: byjus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byjus/refs/heads/main/security/byjus-domain-security.yml
summary_line: DMARC
tags:
- Company
- Edtech
- Education
- E-Learning
- Online Learning
- Tutoring
- Test Prep
- India
- Learning App
---
