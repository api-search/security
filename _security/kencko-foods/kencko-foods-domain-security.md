---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kencko.com
  spf: true
hosts:
- cert_expires: Sep 25 15:46:27 2026 GMT
  host: kencko.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kencko Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kencko Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kencko Foods
provider_slug: kencko-foods
slug: kencko-foods-domain-security
source_filename: kencko-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kencko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:46:27 2026 GMT\n  hsts: null\ndomains:\n- domain: kencko.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kencko-foods/refs/heads/main/security/kencko-foods-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food and Beverage
- Consumer Products
- E-Commerce
- Health and Wellness
- Direct to Consumer
- Shopify
---
