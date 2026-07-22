---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nyansa.com
  spf: true
hosts:
- host: nyansa.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nyansa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nyansa, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nyansa
provider_slug: nyansa
slug: nyansa-domain-security
source_filename: nyansa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nyansa.com\n  https: false\ndomains:\n- domain: nyansa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nyansa/refs/heads/main/security/nyansa-domain-security.yml
summary_line: DMARC
tags:
- Company
---
