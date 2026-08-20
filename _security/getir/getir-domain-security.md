---
api_specs:
- filename: getir-food-openapi.yml
  format: yaml
  label: GetirFood API
  slug: getirfood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/openapi/getir-food-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getir.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: getirapi.com
  spf: false
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: getir.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: developers.getir.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: food-external-api-gateway.getirapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getir, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Getir
provider_slug: getir
slug: getir-domain-security
source_filename: getir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getir.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\n- host: developers.getir.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: food-external-api-gateway.getirapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: getir.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: getirapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getir/refs/heads/main/security/getir-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Delivery
- Grocery Delivery
- On-Demand Delivery
- Logistics
- Restaurant
- Point-of-Sale
- Marketplace
- Turkey
- Partner Integration
---
