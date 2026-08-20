---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coldsnap.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Oct 26 17:59:34 2026 GMT
  host: coldsnap.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:37:15 2026 GMT
  host: shopify.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coldsnap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ColdSnap, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ColdSnap
provider_slug: coldsnap
slug: coldsnap-domain-security
source_filename: coldsnap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coldsnap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 17:59:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: coldsnap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coldsnap/refs/heads/main/security/coldsnap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Food and Beverage
- Consumer Products
- Hardware
- Appliances
- Food Service
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
---
