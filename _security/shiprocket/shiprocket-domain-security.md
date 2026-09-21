---
api_specs:
- filename: shiprocket-api-openapi.yml
  format: yaml
  label: Shiprocket API
  slug: shiprocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiprocket/refs/heads/main/openapi/shiprocket-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "emsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shiprocket.in
  spf: true
hosts:
- cert_expires: Dec 15 23:52:29 2026 GMT
  host: www.shiprocket.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 13:52:15 2026 GMT
  host: apidocs.shiprocket.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: apiv2.shiprocket.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Shiprocket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shiprocket, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shiprocket
provider_slug: shiprocket
slug: shiprocket-domain-security
source_filename: shiprocket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shiprocket.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:52:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.shiprocket.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 13:52:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apiv2.shiprocket.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shiprocket.in\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"emsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiprocket/refs/heads/main/security/shiprocket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Shipping
- Logistics
- E-Commerce
- Fulfillment
- Last Mile Delivery
- Order Management
- Courier Aggregation
- India
---
