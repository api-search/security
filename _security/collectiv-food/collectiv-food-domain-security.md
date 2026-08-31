---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: collectivfood.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: collectivfood.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collectiv Food Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collectiv Food, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Collectiv Food
provider_slug: collectiv-food
slug: collectiv-food-domain-security
source_filename: collectiv-food-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: collectivfood.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: collectivfood.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collectiv-food/refs/heads/main/security/collectiv-food-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Applicative Saas
- Food
- Food Wholesale
- Food Distribution
- Supply Chain
- Foodtech
- Sustainability
- B2B
---
