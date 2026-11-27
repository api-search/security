---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: junkyard.guru
  spf: true
hosts:
- host: junkyard.guru
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: junkyard-guru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for junkyard-guru, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: junkyard-guru
provider_slug: junkyard-guru
slug: junkyard-guru-domain-security
source_filename: junkyard-guru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: junkyard.guru\n  https: false\ndomains:\n- domain: junkyard.guru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/junkyard-guru/security/junkyard-guru-domain-security.yml
summary_line: DMARC
tags:
- Company
---
