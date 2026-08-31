---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: radpowerbikes.com
  spf: true
hosts:
- cert_expires: Oct 23 03:08:31 2026 GMT
  host: www.radpowerbikes.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rad Power Bikes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rad Power Bikes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rad Power Bikes
provider_slug: rad-power-bikes
slug: rad-power-bikes-domain-security
source_filename: rad-power-bikes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.radpowerbikes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 03:08:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: radpowerbikes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rad-power-bikes/refs/heads/main/security/rad-power-bikes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electric Bikes
- Micromobility
- E-Commerce
- Retail
- Consumer Products
- Agentic Commerce
- Shopify
- MCP
- Universal Commerce Protocol
---
