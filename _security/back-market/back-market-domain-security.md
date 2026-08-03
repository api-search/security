---
api_specs:
- filename: back-market-openapi-original.yml
  format: yaml
  label: Back Market API
  slug: back-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/back-market/refs/heads/main/openapi/back-market-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: backmarket.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: backmarket.dev
  spf: false
hosts:
- cert_expires: Oct 15 14:14:57 2026 GMT
  host: www.backmarket.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 22:00:19 2026 GMT
  host: api.backmarket.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 00:04:07 2026 GMT
  host: preprod.backmarket.co.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Back Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Back Market, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Back Market
provider_slug: back-market
slug: back-market-domain-security
source_filename: back-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.backmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:14:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.backmarket.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:00:19 2026 GMT\n  hsts: false\n- host: preprod.backmarket.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:04:07 2026 GMT\n  hsts: null\ndomains:\n- domain: backmarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: backmarket.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/back-market/refs/heads/main/security/back-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Refurbished Electronics
- Circular Economy
- Orders
- Listings
- Product Catalog
- Logistics
- Customer Support
---
