---
api_specs:
- filename: appcharge-assets-api-openapi.yml
  format: yaml
  label: Appcharge Assets API
  slug: appcharge-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-assets-api-openapi.yml
- filename: appcharge-authentication-api-openapi.yml
  format: yaml
  label: Appcharge Authentication API
  slug: appcharge-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-authentication-api-openapi.yml
- filename: appcharge-badges-api-openapi.yml
  format: yaml
  label: Appcharge Badges API
  slug: appcharge-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-badges-api-openapi.yml
- filename: appcharge-coupons-api-openapi.yml
  format: yaml
  label: Appcharge Coupons API
  slug: appcharge-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-coupons-api-openapi.yml
- filename: appcharge-general-api-openapi.yml
  format: yaml
  label: Appcharge General API
  slug: appcharge-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-general-api-openapi.yml
- filename: appcharge-localization-api-openapi.yml
  format: yaml
  label: Appcharge Localization API
  slug: appcharge-localization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-localization-api-openapi.yml
- filename: appcharge-offer-designs-api-openapi.yml
  format: yaml
  label: Appcharge Offer Designs API
  slug: appcharge-offer-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-offer-designs-api-openapi.yml
- filename: appcharge-offers-api-openapi.yml
  format: yaml
  label: Appcharge Offers API
  slug: appcharge-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-offers-api-openapi.yml
- filename: appcharge-orders-api-openapi.yml
  format: yaml
  label: Appcharge Orders API
  slug: appcharge-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-orders-api-openapi.yml
- filename: appcharge-personalization-api-openapi.yml
  format: yaml
  label: Appcharge Personalization API
  slug: appcharge-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-personalization-api-openapi.yml
- filename: appcharge-popups-api-openapi.yml
  format: yaml
  label: Appcharge Popups API
  slug: appcharge-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-popups-api-openapi.yml
- filename: appcharge-portal-content-api-openapi.yml
  format: yaml
  label: Appcharge Portal Content API
  slug: appcharge-portal-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-portal-content-api-openapi.yml
- filename: appcharge-products-api-openapi.yml
  format: yaml
  label: Appcharge Products API
  slug: appcharge-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-products-api-openapi.yml
- filename: appcharge-promo-codes-api-openapi.yml
  format: yaml
  label: Appcharge Promo Codes API
  slug: appcharge-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-promo-codes-api-openapi.yml
- filename: appcharge-rolling-offers-api-openapi.yml
  format: yaml
  label: Appcharge Rolling Offers API
  slug: appcharge-rolling-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-rolling-offers-api-openapi.yml
- filename: appcharge-store-refresh-popups-api-openapi.yml
  format: yaml
  label: Appcharge Store Refresh Popups API
  slug: appcharge-store-refresh-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-store-refresh-popups-api-openapi.yml
- filename: appcharge-triggered-popups-api-openapi.yml
  format: yaml
  label: Appcharge Triggered Popups API
  slug: appcharge-triggered-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/openapi/appcharge-triggered-popups-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appcharge.com
  spf: true
hosts:
- cert_expires: Sep 13 14:58:44 2026 GMT
  host: appcharge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.appcharge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api-sandbox.appcharge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appcharge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appcharge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appcharge
provider_slug: appcharge
slug: appcharge-domain-security
source_filename: appcharge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appcharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.appcharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\n- host: api-sandbox.appcharge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: appcharge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appcharge/refs/heads/main/security/appcharge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Monetization
- Merchant of Record
- Mobile Games
- Gaming
- Checkout
- In-Game Purchases
- Web Store
- E-Commerce
---
