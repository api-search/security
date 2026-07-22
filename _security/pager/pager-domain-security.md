---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pager.xyz
  spf: true
hosts:
- host: www.pager.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: Pager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pager, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pager
provider_slug: pager
slug: pager-domain-security
source_filename: pager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pager.xyz\n  https: false\ndomains:\n- domain: pager.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pager/refs/heads/main/security/pager-domain-security.yml
summary_line: DMARC
tags:
- Company
- Consumer
---
