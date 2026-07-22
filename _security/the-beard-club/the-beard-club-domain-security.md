---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thebeardclub.com
  spf: true
hosts:
- cert_expires: Aug 29 09:18:34 2026 GMT
  host: thebeardclub.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Beard Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Beard Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Beard Club
provider_slug: the-beard-club
slug: the-beard-club-domain-security
source_filename: the-beard-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thebeardclub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 09:18:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: thebeardclub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-beard-club/refs/heads/main/security/the-beard-club-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Retail
- Men's Grooming
- Consumer Goods
- Shopify
- Agent Commerce
- UCP
- MCP
- Subscription
---
