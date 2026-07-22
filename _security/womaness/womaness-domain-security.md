---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: womaness.com
  spf: true
hosts:
- cert_expires: Sep  1 04:43:34 2026 GMT
  host: womaness.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Womaness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Womaness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Womaness
provider_slug: womaness
slug: womaness-domain-security
source_filename: womaness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: womaness.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:43:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: womaness.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/womaness/refs/heads/main/security/womaness-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wellness
- Menopause
- Women's Health
- Skincare
- Supplements
- Direct to Consumer
- Ecommerce
- Shopify
---
