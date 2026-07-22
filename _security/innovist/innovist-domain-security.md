---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: innovist.com
  spf: false
hosts:
- cert_expires: Sep  8 04:51:03 2026 GMT
  host: innovist.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Innovist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Innovist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Innovist
provider_slug: innovist
slug: innovist-domain-security
source_filename: innovist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: innovist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:51:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: innovist.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovist/refs/heads/main/security/innovist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Personal Care
- Skincare
- Haircare
- Suncare
- Direct to Consumer
- Ecommerce
- Shopify
- Agentic Commerce
---
