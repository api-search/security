---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sorrisopharma.com
  spf: true
hosts:
- host: www.sorrisopharma.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sorriso Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sorriso Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sorriso Pharmaceuticals
provider_slug: sorriso-pharmaceuticals
slug: sorriso-pharmaceuticals-domain-security
source_filename: sorriso-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sorrisopharma.com\n  https: false\ndomains:\n- domain: sorrisopharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sorriso-pharmaceuticals/security/sorriso-pharmaceuticals-domain-security.yml
summary_line: DMARC
tags:
- Company
- Biopharma
- Healthcare
- Pharmaceuticals
- Research
---
