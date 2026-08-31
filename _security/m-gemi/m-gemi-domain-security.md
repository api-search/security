---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mgemi.com
  spf: true
hosts:
- cert_expires: Oct 26 17:30:33 2026 GMT
  host: mgemi.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: M Gemi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M.Gemi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: M.Gemi
provider_slug: m-gemi
slug: m-gemi-domain-security
source_filename: m-gemi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mgemi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 17:30:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: mgemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m-gemi/refs/heads/main/security/m-gemi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Fashion
- Footwear
- Direct to Consumer
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Catalog
- Checkout
---
