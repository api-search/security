---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ergooffers.com
  spf: true
hosts:
- host: www.ergooffers.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ergo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ergo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ergo
provider_slug: ergo
slug: ergo-domain-security
source_filename: ergo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ergooffers.com\n  https: false\ndomains:\n- domain: ergooffers.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ergo/refs/heads/main/security/ergo-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- E-Commerce
- Retail
- Pricing
- Shopify
- Analytics
- Merchandising
- Pricing Optimization
---
