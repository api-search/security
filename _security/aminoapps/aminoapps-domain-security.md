---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aminoapps.com
  spf: true
hosts:
- host: aminoapps.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aminoapps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aminoapps, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aminoapps
provider_slug: aminoapps
slug: aminoapps-domain-security
source_filename: aminoapps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aminoapps.com\n  https: false\ndomains:\n- domain: aminoapps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aminoapps/refs/heads/main/security/aminoapps-domain-security.yml
summary_line: DMARC
tags:
- Company
- Social
- Community
- Mobile
- Content
---
