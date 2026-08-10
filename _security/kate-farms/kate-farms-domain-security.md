---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: katefarms.com
  spf: true
hosts:
- cert_expires: Sep  7 08:23:56 2026 GMT
  host: katefarms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 00:18:33 2026 GMT
  host: shop.katefarms.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kate Farms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kate Farms, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Kate Farms
provider_slug: kate-farms
slug: kate-farms-domain-security
source_filename: kate-farms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: katefarms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 08:23:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shop.katefarms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 00:18:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: katefarms.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kate-farms/refs/heads/main/security/kate-farms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Nutrition
- Medical Nutrition
- Health
- Food and Beverage
- Consumer Packaged Goods
- E-Commerce
- Agentic Commerce
- Retail
- Shopify
- GraphQL
---
