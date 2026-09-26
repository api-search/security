---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daring.com
  spf: true
hosts:
- cert_expires: Sep 23 19:32:59 2026 GMT
  host: daring.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Daring Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daring Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daring Foods
provider_slug: daring-foods
slug: daring-foods-domain-security
source_filename: daring-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:32:59 2026 GMT\n  hsts: null\ndomains:\n- domain: daring.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/security/daring-foods-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- Consumer Packaged Goods
- Plant-Based
- Alternative Protein
- Food and Beverage
- Recipes
- Food Service
- Grocery
---
