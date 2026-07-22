---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ttracing.my
  spf: false
hosts:
- cert_expires: Aug 24 23:54:02 2026 GMT
  host: ttracing.my
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ttracing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TTRacing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TTRacing
provider_slug: ttracing
slug: ttracing-domain-security
source_filename: ttracing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ttracing.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:54:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: ttracing.my\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ttracing/refs/heads/main/security/ttracing-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming Chairs
- Gaming Furniture
- Ecommerce
- Retail
- Agent Commerce
- MCP
- Shopify
- Malaysia
---
