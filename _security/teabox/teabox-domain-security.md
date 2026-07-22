---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: teabox.com
  spf: true
hosts:
- cert_expires: Aug 26 08:16:33 2026 GMT
  host: www.teabox.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teabox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teabox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Teabox
provider_slug: teabox
slug: teabox-domain-security
source_filename: teabox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teabox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 08:16:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: teabox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teabox/refs/heads/main/security/teabox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Tea
- Food and Beverage
- E-commerce
- Retail
- Shopify
- Agent Commerce
---
