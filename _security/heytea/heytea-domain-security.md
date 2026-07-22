---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heytea.com
  spf: true
hosts:
- host: heytea.com
  https: false
kind: domain-security
layout: security
method: probed
name: Heytea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heytea, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Heytea
provider_slug: heytea
slug: heytea-domain-security
source_filename: heytea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heytea.com\n  https: false\ndomains:\n- domain: heytea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heytea/refs/heads/main/security/heytea-domain-security.yml
summary_line: DMARC
tags:
- Company
- Consumer
- Food and Beverage
- Beverages
- Tea
- Retail
- China
---
