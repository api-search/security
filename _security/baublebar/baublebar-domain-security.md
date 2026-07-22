---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: baublebar.com
  spf: true
hosts:
- cert_expires: Sep 10 14:17:44 2026 GMT
  host: www.baublebar.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baublebar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BaubleBar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BaubleBar
provider_slug: baublebar
slug: baublebar-domain-security
source_filename: baublebar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baublebar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:17:44 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: baublebar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baublebar/refs/heads/main/security/baublebar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Retail
- E-commerce
- Jewelry
- Accessories
- Fashion
- Shopify
- MCP
---
