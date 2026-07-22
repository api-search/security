---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tothemarket.com
  spf: true
hosts:
- cert_expires: Aug 29 02:04:33 2026 GMT
  host: tothemarket.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: To The Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TO THE MARKET, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TO THE MARKET
provider_slug: to-the-market
slug: to-the-market-domain-security
source_filename: to-the-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tothemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:04:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: tothemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/to-the-market/refs/heads/main/security/to-the-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- Ecommerce
- Sustainability
- Supply Chain
- Agent Commerce
- Shopify
- MCP
---
