---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pango.ai
  spf: true
hosts:
- cert_expires: Aug 18 16:07:58 2026 GMT
  host: pango.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pango Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pango, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pango
provider_slug: pango
slug: pango-domain-security
source_filename: pango-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pango.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:07:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pango.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pango/refs/heads/main/security/pango-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-Commerce
- Logistics
- Shipping
- Fulfillment
- Returns
- Order Tracking
- Artificial Intelligence
- Agents
- Y Combinator
---
