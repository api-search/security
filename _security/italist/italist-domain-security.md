---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: italist.com
  spf: true
hosts:
- cert_expires: Aug 29 15:18:05 2026 GMT
  host: italist.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Italist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Italist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Italist
provider_slug: italist
slug: italist-domain-security
source_filename: italist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: italist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 15:18:05 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: italist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/italist/refs/heads/main/security/italist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Retail
- Fashion
- Luxury
- Marketplace
- Shopify
- Agentic Commerce
- MCP
---
