---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bestprice.gr
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.bestprice.gr
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: mcp.bestprice.gr
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bestprice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BestPrice Agent Commerce, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BestPrice Agent Commerce
provider_slug: bestprice
slug: bestprice-domain-security
source_filename: bestprice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bestprice.gr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\n- host: mcp.bestprice.gr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bestprice.gr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bestprice/refs/heads/main/security/bestprice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shopping
- Price Comparison
- E-Commerce
- Retail
- MCP
- WebMCP
- Agent Commerce
- Greece
---
