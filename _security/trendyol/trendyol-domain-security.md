---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trendyol.com
  spf: true
hosts:
- cert_expires: Nov 10 10:44:30 2026 GMT
  host: trendyol.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 12:47:09 2026 GMT
  host: developers.trendyol.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 10:44:30 2026 GMT
  host: apigw.trendyol.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trendyol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trendyol, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trendyol
provider_slug: trendyol
slug: trendyol-domain-security
source_filename: trendyol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trendyol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 10:44:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developers.trendyol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 12:47:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apigw.trendyol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 10:44:30 2026 GMT\n  hsts: null\ndomains:\n- domain: trendyol.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trendyol/refs/heads/main/security/trendyol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Marketplace
- Retail
- Fashion
- Turkey
- Order Management
- Fulfillment
- Logistics
- Webhooks
---
