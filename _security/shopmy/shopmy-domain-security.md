---
api_specs:
- filename: shopmy-catalog-api-openapi.yml
  format: yaml
  label: ShopMy Catalog API
  slug: shopmy-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/openapi/shopmy-catalog-api-openapi.yml
- filename: shopmy-collections-api-openapi.yml
  format: yaml
  label: ShopMy Collections API
  slug: shopmy-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/openapi/shopmy-collections-api-openapi.yml
- filename: shopmy-links-api-openapi.yml
  format: yaml
  label: ShopMy Links API
  slug: shopmy-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/openapi/shopmy-links-api-openapi.yml
- filename: shopmy-oauth-api-openapi.yml
  format: yaml
  label: ShopMy OAuth API
  slug: shopmy-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/openapi/shopmy-oauth-api-openapi.yml
- filename: shopmy-order-reporting-api-openapi.yml
  format: yaml
  label: ShopMy Order Reporting API
  slug: shopmy-order-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/openapi/shopmy-order-reporting-api-openapi.yml
- filename: shopmy-profile-api-openapi.yml
  format: yaml
  label: ShopMy Profile API
  slug: shopmy-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/openapi/shopmy-profile-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shopmy.us
  spf: true
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: shopmy.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopmy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShopMy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShopMy
provider_slug: shopmy
slug: shopmy-domain-security
source_filename: shopmy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shopmy.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: shopmy.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/security/shopmy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Commerce
- Creator Economy
- Creator Commerce
- Affiliate Marketing
- Influencer Marketing
- E-Commerce
- Retail
---
