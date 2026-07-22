---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: edgar-online.com
  spf: true
hosts:
- host: edgar-online.com
  https: false
kind: domain-security
layout: security
method: probed
name: Edgar Online Otc Markets Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edgar Online (OTC Markets Group), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Edgar Online (OTC Markets Group)
provider_slug: edgar-online-otc-markets-group
slug: edgar-online-otc-markets-group-domain-security
source_filename: edgar-online-otc-markets-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edgar-online.com\n  https: false\ndomains:\n- domain: edgar-online.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgar-online-otc-markets-group/refs/heads/main/security/edgar-online-otc-markets-group-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fintech
- Financial Data
- SEC Filings
- Market Data
- Securities
---
