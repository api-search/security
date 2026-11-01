---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: waterfall.market
  spf: true
hosts:
- host: www.waterfall.market
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Waterfall Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waterfall, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Waterfall
provider_slug: waterfall-market
slug: waterfall-market-domain-security
source_filename: waterfall-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.waterfall.market\n  https: false\ndomains:\n- domain: waterfall.market\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/waterfall-market/security/waterfall-market-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Marketplace
- Procurement
- SaaS
- API
---
