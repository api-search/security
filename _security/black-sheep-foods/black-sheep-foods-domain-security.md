---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blacksheepfoods.com
  spf: true
hosts:
- cert_expires: Sep 10 19:47:33 2026 GMT
  host: blacksheepfoods.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Sheep Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Sheep Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Black Sheep Foods
provider_slug: black-sheep-foods
slug: black-sheep-foods-domain-security
source_filename: black-sheep-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blacksheepfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 19:47:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: blacksheepfoods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-sheep-foods/refs/heads/main/security/black-sheep-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Deep Tech
- Food Technology
- Plant-Based Meat
- Alternative Protein
- Food and Beverage
- Consumer Packaged Goods
- Sustainability
---
