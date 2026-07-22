---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monsanto.com
  spf: true
hosts:
- host: www.monsanto.com
  https: false
kind: domain-security
layout: security
method: probed
name: Monsanto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monsanto, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Monsanto
provider_slug: monsanto
slug: monsanto-domain-security
source_filename: monsanto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monsanto.com\n  https: false\ndomains:\n- domain: monsanto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monsanto/refs/heads/main/security/monsanto-domain-security.yml
summary_line: DMARC
tags:
- Agriculture
- Biotechnology
- Crop Science
- Seeds
- Fortune 500
---
