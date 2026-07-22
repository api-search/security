---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: searchlight.ai
  spf: true
hosts:
- host: www.searchlight.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Searchlight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Searchlight, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Searchlight
provider_slug: searchlight
slug: searchlight-domain-security
source_filename: searchlight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.searchlight.ai\n  https: false\ndomains:\n- domain: searchlight.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchlight/refs/heads/main/security/searchlight-domain-security.yml
summary_line: DMARC
tags:
- Company
- Services
- Startup
- SaaS
- Accel
- Web Application
---
