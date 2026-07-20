---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: easysize.me
  spf: true
hosts:
- cert_expires: Sep 18 14:44:45 2026 GMT
  host: easysize.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 01:56:17 2026 GMT
  host: developers.easysize.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: webapp.easysize.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Easysize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EasySize, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EasySize
provider_slug: easysize
slug: easysize-domain-security
source_filename: easysize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easysize.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:44:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.easysize.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:56:17 2026 GMT\n  hsts: false\n- host: webapp.easysize.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: easysize.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easysize/refs/heads/main/security/easysize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- E-Commerce
- Size Recommendation
- Fit
- Retail
- Shopify
- Personalization
- Widget
- JavaScript
---
