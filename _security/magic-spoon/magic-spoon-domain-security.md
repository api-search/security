---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magicspoon.com
  spf: true
hosts:
- cert_expires: Aug 28 12:22:32 2026 GMT
  host: magicspoon.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magic Spoon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic Spoon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Magic Spoon
provider_slug: magic-spoon
slug: magic-spoon-domain-security
source_filename: magic-spoon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magicspoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:22:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: magicspoon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-spoon/refs/heads/main/security/magic-spoon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Ecommerce
- Food and Beverage
- Direct to Consumer
- Retail
- Subscription
---
