---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: johnnie-o.com
  spf: true
hosts:
- cert_expires: Sep 27 04:13:02 2026 GMT
  host: www.johnnie-o.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 11:54:02 2026 GMT
  host: checkout.johnnie-o.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Johnnie O Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Johnnie-O, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Johnnie-O
provider_slug: johnnie-o
slug: johnnie-o-domain-security
source_filename: johnnie-o-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.johnnie-o.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: checkout.johnnie-o.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 11:54:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: johnnie-o.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johnnie-o/refs/heads/main/security/johnnie-o-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Apparel
- Retail
- E-Commerce
- Direct to Consumer
- Golf
- Fashion
- Consumer Goods
- Shopify
- Agentic Commerce
---
