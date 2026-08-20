---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crukafe.com
  spf: true
hosts:
- cert_expires: Aug 29 06:42:34 2026 GMT
  host: crukafe.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cru Kafe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CRU Kafe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CRU Kafe
provider_slug: cru-kafe
slug: cru-kafe-domain-security
source_filename: cru-kafe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crukafe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:42:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: crukafe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cru-kafe/refs/heads/main/security/cru-kafe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coffee
- E-Commerce
- Retail
- Consumer Goods
- Food and Beverage
- Shopify
- Agent Commerce
- UCP
---
