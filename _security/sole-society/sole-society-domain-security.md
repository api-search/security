---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solesociety.com
  spf: true
hosts:
- host: www.solesociety.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sole Society Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sole Society, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sole Society
provider_slug: sole-society
slug: sole-society-domain-security
source_filename: sole-society-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solesociety.com\n  https: false\ndomains:\n- domain: solesociety.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sole-society/refs/heads/main/security/sole-society-domain-security.yml
summary_line: DMARC
tags:
- Company
- Footwear
- Fashion
- Ecommerce
- Retail
- Accessories
- Handbags
---
