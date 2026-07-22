---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: resourcely.io
  spf: true
hosts:
- host: www.resourcely.io
  https: false
kind: domain-security
layout: security
method: probed
name: Resourcely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resourcely, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Resourcely
provider_slug: resourcely
slug: resourcely-domain-security
source_filename: resourcely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.resourcely.io\n  https: false\ndomains:\n- domain: resourcely.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resourcely/refs/heads/main/security/resourcely-domain-security.yml
summary_line: DMARC
tags:
- Company
- Startup
- Venture Backed
- a16z
- Portfolio
---
