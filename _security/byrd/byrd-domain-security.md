---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:incidents@getbyrd.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getbyrd.com
  spf: true
hosts:
- cert_expires: Oct 14 21:37:41 2026 GMT
  host: www.getbyrd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 04:20:22 2026 GMT
  host: developers.getbyrd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 10:32:32 2026 GMT
  host: api.getbyrd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Byrd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Byrd, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Byrd
provider_slug: byrd
slug: byrd-domain-security
source_filename: byrd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getbyrd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:37:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.getbyrd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:20:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getbyrd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:32:32 2026 GMT\n  hsts: null\ndomains:\n- domain: getbyrd.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:incidents@getbyrd.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byrd/refs/heads/main/security/byrd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E-Commerce
- Fulfillment
- Logistics
- 3PL
- Shipping
- Warehousing
- Order Management
- Inventory
- Returns
- Supply Chain
---
