---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getshogun.com
  spf: true
hosts:
- cert_expires: Oct  8 20:43:03 2026 GMT
  host: getshogun.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shogun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shogun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shogun
provider_slug: shogun
slug: shogun-domain-security
source_filename: shogun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getshogun.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 20:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: getshogun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shogun/refs/heads/main/security/shogun-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Page Builder
- Headless Commerce
- Shopify
- BigCommerce
- Conversion Optimization
- No-Code
---
