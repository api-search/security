---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: numitea.com
  spf: true
hosts:
- cert_expires: Nov 14 01:29:34 2026 GMT
  host: numitea.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Numi Tea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numi Tea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Numi Tea
provider_slug: numi-tea
slug: numi-tea-domain-security
source_filename: numi-tea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numitea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 01:29:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: numitea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numi-tea/refs/heads/main/security/numi-tea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tea
- Beverages
- Consumer Packaged Goods
- Retail
- E-Commerce
- Organic
- Fair Trade
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
---
