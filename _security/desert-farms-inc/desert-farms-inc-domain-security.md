---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: desertfarms.com
  spf: true
hosts:
- cert_expires: Aug 28 22:53:31 2026 GMT
  host: desertfarms.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Desert Farms Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DESERT FARMS INC., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DESERT FARMS INC.
provider_slug: desert-farms-inc
slug: desert-farms-inc-domain-security
source_filename: desert-farms-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: desertfarms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:53:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: desertfarms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/desert-farms-inc/refs/heads/main/security/desert-farms-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Camel Milk
- Consumer Packaged Goods
- E-Commerce
- Food and Beverage
- Direct to Consumer
- Shopify
- Retail
---
