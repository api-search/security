---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newegg.com
  spf: true
hosts:
- cert_expires: Aug 29 05:09:30 2026 GMT
  host: www.newegg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 16:03:55 2026 GMT
  host: developer.newegg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 05:09:30 2026 GMT
  host: api.newegg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newegg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newegg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Newegg
provider_slug: newegg
slug: newegg-domain-security
source_filename: newegg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newegg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:09:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.newegg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.newegg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:09:30 2026 GMT\n  hsts: null\ndomains:\n- domain: newegg.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newegg/refs/heads/main/security/newegg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- E-Commerce
- Marketplace
- Retail
- Electronics
- Sellers
- Order Management
- Fulfillment
---
