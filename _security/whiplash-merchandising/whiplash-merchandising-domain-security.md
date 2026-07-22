---
api_specs:
- filename: whiplash-merchandising-openapi-original.json
  format: json
  label: Rydership API V2
  slug: rydership-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whiplash-merchandising/refs/heads/main/openapi/whiplash-merchandising-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: whiplash.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getwhiplash.com
  spf: false
hosts:
- host: whiplash.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''whiplash.co'
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: developers.getwhiplash.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: www.getwhiplash.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Whiplash Merchandising Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whiplash Merchandising, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Whiplash Merchandising
provider_slug: whiplash-merchandising
slug: whiplash-merchandising-domain-security
source_filename: whiplash-merchandising-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whiplash.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''whiplash.co'\n  hsts: null\n- host: developers.getwhiplash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n- host: www.getwhiplash.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: whiplash.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: getwhiplash.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whiplash-merchandising/refs/heads/main/security/whiplash-merchandising-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fulfillment
- Logistics
- Ecommerce
- Shipping
- Warehousing
- Inventory
- 3PL
- Order Management
- Returns
- Supply Chain
---
