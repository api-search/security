---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mayhem.gg
  spf: false
hosts:
- host: www.mayhem.gg
  https: false
kind: domain-security
layout: security
method: probed
name: Mayhem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mayhem, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Mayhem
provider_slug: mayhem
slug: mayhem-domain-security
source_filename: mayhem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mayhem.gg\n  https: false\ndomains:\n- domain: mayhem.gg\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mayhem/refs/heads/main/security/mayhem-domain-security.yml
summary_line: DMARC
tags:
- Company
- Consumer
---
