---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: walkerandcompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getbevel.com
  spf: true
hosts:
- cert_expires: Sep  9 02:18:39 2026 GMT
  host: walkerandcompany.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 07:38:02 2026 GMT
  host: getbevel.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walkerco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WalkerCo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WalkerCo
provider_slug: walkerco
slug: walkerco-domain-security
source_filename: walkerco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: walkerandcompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 02:18:39 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: getbevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:38:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: walkerandcompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: getbevel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walkerco/refs/heads/main/security/walkerco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health and Beauty
- Consumer Products
- Ecommerce
- Grooming
- Personal Care
- Shopify
- Direct to Consumer
---
