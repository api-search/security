---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tecovas.com
  spf: true
hosts:
- cert_expires: Sep 26 23:13:02 2026 GMT
  host: www.tecovas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 19:47:32 2026 GMT
  host: checkout.tecovas.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tecovas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tecovas, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tecovas
provider_slug: tecovas
slug: tecovas-domain-security
source_filename: tecovas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tecovas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: checkout.tecovas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:47:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: tecovas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tecovas/refs/heads/main/security/tecovas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Footwear
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Product Catalog
---
