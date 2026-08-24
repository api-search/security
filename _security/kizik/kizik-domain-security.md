---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kizik.com
  spf: true
hosts:
- cert_expires: Oct 26 22:34:02 2026 GMT
  host: kizik.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kizik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kizik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kizik
provider_slug: kizik
slug: kizik-domain-security
source_filename: kizik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kizik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 22:34:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: kizik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kizik/refs/heads/main/security/kizik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Footwear
- Consumer Goods
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Direct to Consumer
---
