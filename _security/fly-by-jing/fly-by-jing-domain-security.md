---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flybyjing.com
  spf: false
hosts:
- cert_expires: Aug 31 09:20:03 2026 GMT
  host: flybyjing.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fly By Jing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fly By Jing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Fly By Jing
provider_slug: fly-by-jing
slug: fly-by-jing-domain-security
source_filename: fly-by-jing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flybyjing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:20:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: flybyjing.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fly-by-jing/refs/heads/main/security/fly-by-jing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- E-Commerce
- Shopify
- Direct to Consumer
- MCP
- Agentic Commerce
---
