---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drinkolipop.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Oct 26 05:39:02 2026 GMT
  host: drinkolipop.com
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
name: Olipop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Olipop, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Olipop
provider_slug: olipop
slug: olipop-domain-security
source_filename: olipop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drinkolipop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 05:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: drinkolipop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olipop/refs/heads/main/security/olipop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Beverage
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Retail
- Agent Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- Shopify
- prebiotic-soda
- Functional Beverage
---
