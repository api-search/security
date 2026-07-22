---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: helloyumi.com
  spf: true
hosts:
- cert_expires: Oct  2 23:40:40 2026 GMT
  host: helloyumi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Caer
provider_slug: caer
slug: caer-domain-security
source_filename: caer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helloyumi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:40:40 2026 GMT\n  hsts: false\ndomains:\n- domain: helloyumi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caer/refs/heads/main/security/caer-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- E-commerce
- Baby and Kids
- Nutrition
- Direct to Consumer
- Subscription
---
