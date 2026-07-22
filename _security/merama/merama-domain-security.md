---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: merama.io
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.merama.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Merama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for merama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: merama
provider_slug: merama
slug: merama-domain-security
source_filename: merama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.merama.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: merama.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merama/refs/heads/main/security/merama-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- E-Commerce
- Latin America
- Brand Aggregator
- Marketplace
- Retail
- Investment
---
