---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fnatic.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Oct 17 06:20:04 2026 GMT
  host: fnatic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:37:15 2026 GMT
  host: shopify.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 12:19:03 2026 GMT
  host: shop.fnatic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fnatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fnatic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fnatic
provider_slug: fnatic
slug: fnatic-domain-security
source_filename: fnatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fnatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 06:20:04 2026 GMT\n  hsts: null\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: null\n- host: shop.fnatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 12:19:03 2026 GMT\n  hsts: null\ndomains:\n- domain: fnatic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fnatic/refs/heads/main/security/fnatic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Esports
- Gaming
- Entertainment
- Sports
- Consumer Electronics
- Gaming Hardware
- Apparel
- Ecommerce
- Direct to Consumer
- Agentic Commerce
- Shopify
- GraphQL
- Universal Commerce Protocol
- Model Context Protocol
- United Kingdom
---
