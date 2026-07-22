---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: epizyme.com
  spf: true
hosts:
- host: www.epizyme.com
  https: false
kind: domain-security
layout: security
method: probed
name: Epizyme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epizyme, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Epizyme
provider_slug: epizyme
slug: epizyme-domain-security
source_filename: epizyme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epizyme.com\n  https: false\ndomains:\n- domain: epizyme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epizyme/refs/heads/main/security/epizyme-domain-security.yml
summary_line: DMARC
tags:
- Company
- Healthcare
- Biotechnology
- Pharmaceuticals
- Oncology
- Epigenetics
---
