---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drinkhint.com
  spf: true
hosts:
- cert_expires: Oct 25 18:22:02 2026 GMT
  host: www.drinkhint.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hint
provider_slug: hint
slug: hint-domain-security
source_filename: hint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drinkhint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 18:22:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: drinkhint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hint/refs/heads/main/security/hint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beverages
- Consumer Packaged Goods
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
---
