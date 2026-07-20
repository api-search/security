---
api_specs:
- filename: tiktok-shop-open
  format: yaml
  label: TikTok Shop Open API
  slug: open-api
  spec_type: Postman
  url: https://www.postman.com/tiktok-shop-open
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tiktok.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tiktokshop.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: shop.tiktok.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: partner.tiktokshop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: open-api.tiktokglobalshop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiktok Shop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TikTok Shop API, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TikTok Shop API
provider_slug: tiktok-shop
slug: tiktok-shop-domain-security
source_filename: tiktok-shop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shop.tiktok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n- host: partner.tiktokshop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: null\n- host: open-api.tiktokglobalshop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tiktok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tiktokshop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiktok-shop/refs/heads/main/security/tiktok-shop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-commerce
- Marketplace
- Social Commerce
- Order Management
- Product Catalog
- Fulfillment
---
