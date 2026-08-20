---
api_specs:
- filename: famous-spring-api-swagger.json
  format: json
  label: Spring Seller API
  slug: spring-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/famous/refs/heads/main/openapi/famous-spring-api-swagger.json
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amaze.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teespring.com
  spf: true
hosts:
- cert_expires: Oct 13 22:31:48 2026 GMT
  host: amaze.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 19:28:04 2026 GMT
  host: api.teespring.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Famous Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Famous, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Famous
provider_slug: famous
slug: famous-domain-security
source_filename: famous-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amaze.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 22:31:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.teespring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:28:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amaze.co\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: teespring.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/famous/refs/heads/main/security/famous-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Economy
- Commerce
- Live Shopping
- Media
- E-Commerce
- Marketing
- Print on Demand
- Merchandise
- Storefronts
- Order
- Payouts
---
