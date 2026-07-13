---
api_specs:
- filename: amazon-seller-central-openapi.yml
  format: yaml
  label: Amazon Selling Partner API (SP-API)
  slug: sp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-seller-central/refs/heads/main/openapi/amazon-seller-central-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonservices.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: developer.amazonservices.com
  hsts: true
  hsts_max_age: 47474747
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: developer-docs.amazon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: sellingpartnerapi-na.amazon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Seller Central Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Selling Partner API, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Selling Partner API
provider_slug: amazon-seller-central
slug: amazon-seller-central-domain-security
source_filename: amazon-seller-central-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.amazonservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47474747\n- host: developer-docs.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sellingpartnerapi-na.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazonservices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-seller-central/refs/heads/main/security/amazon-seller-central-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eCommerce
- Marketplace
- Selling Partner
- Amazon
- Seller Central
- Catalog
- Orders
- Inventory
- Fulfillment
---
