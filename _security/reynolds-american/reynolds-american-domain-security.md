---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reynolds-american.com
  spf: false
hosts:
- host: www.reynolds-american.com
  https: false
kind: domain-security
layout: security
method: probed
name: Reynolds American Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reynolds American, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Reynolds American
provider_slug: reynolds-american
slug: reynolds-american-domain-security
source_filename: reynolds-american-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reynolds-american.com\n  https: false\ndomains:\n- domain: reynolds-american.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reynolds-american/refs/heads/main/security/reynolds-american-domain-security.yml
summary_line: DMARC
tags:
- Tobacco
- Consumer Goods
- Fortune 500
- British American Tobacco
---
