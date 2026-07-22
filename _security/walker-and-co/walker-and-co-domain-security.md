---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getbevel.com
  spf: true
hosts:
- cert_expires: Sep  9 07:38:02 2026 GMT
  host: getbevel.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walker And Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walker & Co., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Walker & Co.
provider_slug: walker-and-co
slug: walker-and-co-domain-security
source_filename: walker-and-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:38:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: getbevel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walker-and-co/refs/heads/main/security/walker-and-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Health and Beauty
- Personal Care
- Grooming
- Ecommerce
- Direct to Consumer
- Shopify
---
