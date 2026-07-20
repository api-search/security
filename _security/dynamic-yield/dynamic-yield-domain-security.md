---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dynamicyield.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dy.dev
  spf: true
hosts:
- cert_expires: Oct 15 11:30:14 2026 GMT
  host: www.dynamicyield.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 07:16:49 2026 GMT
  host: dy.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: dy-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dynamic Yield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynamic Yield, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dynamic Yield
provider_slug: dynamic-yield
slug: dynamic-yield-domain-security
source_filename: dynamic-yield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dynamicyield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:30:14 2026 GMT\n  hsts: false\n- host: dy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:16:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dy-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dynamicyield.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dy.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/security/dynamic-yield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Personalization
- Experience Optimization
- Recommendations
- A/B Testing
- Search
- eCommerce
- Retail
- Machine Learning
- MACH
- Mastercard
---
