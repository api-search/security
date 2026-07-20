---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linsyhome.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linsy.com
  spf: true
hosts:
- cert_expires: Sep  7 04:13:06 2026 GMT
  host: www.linsyhome.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 16:01:02 2026 GMT
  host: linsy.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linsy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Linsy
provider_slug: linsy
slug: linsy-domain-security
source_filename: linsy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.linsyhome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 04:13:06 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: linsy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 16:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: linsyhome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: linsy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linsy/refs/heads/main/security/linsy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Furniture
- Home Goods
- Direct To Consumer
- Agentic Commerce
- Shopify
- MCP
---
