---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: talpy.ai
  spf: true
hosts:
- host: talpy.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: talpy-ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for talpy-ai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: talpy-ai
provider_slug: talpy-ai
slug: talpy-ai-domain-security
source_filename: talpy-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talpy.ai\n  https: false\ndomains:\n- domain: talpy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/talpy-ai/security/talpy-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
---
