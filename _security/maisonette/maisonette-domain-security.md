---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: maisonette.com
  spf: true
hosts:
- cert_expires: Sep 25 12:48:31 2026 GMT
  host: www.maisonette.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maisonette Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maisonette, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Maisonette
provider_slug: maisonette
slug: maisonette-domain-security
source_filename: maisonette-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.maisonette.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:48:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: maisonette.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maisonette/refs/heads/main/security/maisonette-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Marketplace
- Shopping
- Children
- Baby
- Apparel
- Home
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
---
