---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: taxatech.com
  spf: false
hosts:
- host: taxatech.com
  https: false
kind: domain-security
layout: security
method: probed
name: Taxa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taxa, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Taxa
provider_slug: taxa
slug: taxa-domain-security
source_filename: taxa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taxatech.com\n  https: false\ndomains:\n- domain: taxatech.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taxa/refs/heads/main/security/taxa-domain-security.yml
summary_line: DMARC
tags:
- Company
- Frontier
- Biotechnology
- Synthetic Biology
- Microbiome
- Skin Care
- Consumer Health
- Probiotics
- Deodorant
---
