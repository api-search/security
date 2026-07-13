---
api_specs:
- filename: best-buy-products-api.yaml
  format: yaml
  label: Best Buy Products API
  slug: products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-products-api.yaml
- filename: best-buy-stores-api.yaml
  format: yaml
  label: Best Buy Stores API
  slug: stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-stores-api.yaml
- filename: best-buy-recommendations-api.yaml
  format: yaml
  label: Best Buy Recommendations API
  slug: recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/openapi/best-buy-recommendations-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bestbuy.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.bestbuy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 07:11:54 2026 GMT
  host: api.bestbuy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Best Buy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Best Buy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Best Buy
provider_slug: best-buy
slug: best-buy-domain-security
source_filename: best-buy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bestbuy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\n- host: api.bestbuy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 07:11:54 2026 GMT\n  hsts: null\ndomains:\n- domain: bestbuy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/security/best-buy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 100
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
---
