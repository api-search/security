---
api_specs:
- filename: flower-shop-network-openapi.yml
  format: yaml
  label: Flower Shop Network JSON API
  slug: flower-shop-network-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flower-shop-network/refs/heads/main/openapi/flower-shop-network-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowershopnetwork.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.flowershopnetwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: api.flowershopnetwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: dev-api.flowershopnetwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flower Shop Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flower Shop Network, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flower Shop Network
provider_slug: flower-shop-network
slug: flower-shop-network-domain-security
source_filename: flower-shop-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flowershopnetwork.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flowershopnetwork.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev-api.flowershopnetwork.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowershopnetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flower-shop-network/refs/heads/main/security/flower-shop-network-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Florists
- Flowers
- Wire Orders
- Point of Sale
---
