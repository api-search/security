---
api_specs:
- filename: newstore-api-openapi-original.json
  format: json
  label: NewStore Omnichannel API
  slug: newstore-omnichannel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/openapi/newstore-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: newstore.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newstore.net
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: developer.newstore.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: dodici-demo.p.newstore.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newstore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newstore, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Newstore
provider_slug: newstore
slug: newstore-domain-security
source_filename: newstore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.newstore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dodici-demo.p.newstore.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: newstore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: newstore.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/security/newstore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Omnichannel
- Order Management
- Point of Sale
- Ecommerce
- Fulfillment
- Inventory
- Store Operations
- REST
---
