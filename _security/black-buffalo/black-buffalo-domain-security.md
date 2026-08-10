---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blackbuffalo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Oct 25 10:25:01 2026 GMT
  host: blackbuffalo.com
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
- cert_expires: Sep  6 11:38:51 2026 GMT
  host: ucp.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Buffalo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Buffalo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Black Buffalo
provider_slug: black-buffalo
slug: black-buffalo-domain-security
source_filename: black-buffalo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackbuffalo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 10:25:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: ucp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 11:38:51 2026 GMT\n  hsts: false\ndomains:\n- domain: blackbuffalo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-buffalo/refs/heads/main/security/black-buffalo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Nicotine Pouches
- Smokeless Tobacco Alternative
- Ecommerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- GraphQL
- Model Context Protocol
- Universal Commerce Protocol
---
