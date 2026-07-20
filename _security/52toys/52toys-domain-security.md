---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 52toys.com
  spf: false
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: 52toys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 52Toys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 52TOYS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 52TOYS
provider_slug: 52toys
slug: 52toys-domain-security
source_filename: 52toys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 52toys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: 52toys.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/52toys/refs/heads/main/security/52toys-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Collectibles
- Toys
- Retail
- Ecommerce
- Shopify
- Agentic Commerce
---
