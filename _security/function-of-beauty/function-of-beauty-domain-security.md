---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: functionofbeauty.com
  spf: true
hosts:
- cert_expires: Sep 17 03:08:32 2026 GMT
  host: functionofbeauty.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Function Of Beauty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Function of Beauty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Function of Beauty
provider_slug: function-of-beauty
slug: function-of-beauty-domain-security
source_filename: function-of-beauty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: functionofbeauty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:08:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: functionofbeauty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/function-of-beauty/refs/heads/main/security/function-of-beauty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Beauty
- Personal Care
- Personalization
- E-Commerce
- Shopify
- Direct to Consumer
- MCP
---
