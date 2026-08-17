---
api_specs:
- filename: antavo-events-openapi.yml
  format: yaml
  label: Antavo Events API
  slug: antavo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-events-openapi.yml
- filename: antavo-async-events-openapi.yml
  format: yaml
  label: Antavo Async Events API
  slug: antavo-async-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-async-events-openapi.yml
- filename: antavo-customer-openapi.yml
  format: yaml
  label: Antavo Customer API
  slug: antavo-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-customer-openapi.yml
- filename: antavo-display-openapi.yml
  format: yaml
  label: Antavo Display API
  slug: antavo-display-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-display-openapi.yml
- filename: antavo-entities-openapi.yml
  format: yaml
  label: Antavo Entities API
  slug: antavo-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-entities-openapi.yml
- filename: antavo-rewards-openapi.yml
  format: yaml
  label: Antavo Rewards API
  slug: antavo-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-rewards-openapi.yml
- filename: antavo-coupons-openapi.yml
  format: yaml
  label: Antavo Coupons and Coupon Pools API
  slug: antavo-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-coupons-openapi.yml
- filename: antavo-offers-openapi.yml
  format: yaml
  label: Antavo Offers API
  slug: antavo-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-offers-openapi.yml
- filename: antavo-points-preview-openapi.yml
  format: yaml
  label: Antavo Points Preview API
  slug: antavo-points-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-points-preview-openapi.yml
- filename: antavo-leaderboard-openapi.yml
  format: yaml
  label: Antavo Leaderboard API
  slug: antavo-leaderboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-leaderboard-openapi.yml
- filename: antavo-bulk-operations-openapi.yml
  format: yaml
  label: Antavo Bulk Operations API
  slug: antavo-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-bulk-operations-openapi.yml
- filename: antavo-clubs-openapi.yml
  format: yaml
  label: Antavo Clubs API
  slug: antavo-clubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-clubs-openapi.yml
- filename: antavo-promotion-engine-openapi.yml
  format: yaml
  label: Antavo Promotion Engine API
  slug: antavo-promotion-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-promotion-engine-openapi.yml
- filename: antavo-authentication-openapi.yml
  format: yaml
  label: Antavo Authentication API
  slug: antavo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-authentication-openapi.yml
- filename: antavo-faq-openapi.yml
  format: yaml
  label: Antavo FAQ API
  slug: antavo-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-faq-openapi.yml
- filename: antavo-loyalty-read-openapi.yml
  format: yaml
  label: Antavo Loyalty Read API
  slug: antavo-loyalty-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-loyalty-read-openapi.yml
- filename: antavo-social-share-campaigns-openapi.yml
  format: yaml
  label: Antavo Social Share Campaigns API
  slug: antavo-social-share-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-social-share-campaigns-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: antavo.com
  spf: true
hosts:
- cert_expires: Oct 15 22:49:28 2026 GMT
  host: antavo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 10:50:42 2026 GMT
  host: developers.antavo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 21:13:31 2026 GMT
  host: api.antavo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antavo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antavo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Antavo
provider_slug: antavo
slug: antavo-domain-security
source_filename: antavo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 22:49:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.antavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 10:50:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.antavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:13:31 2026 GMT\n  hsts: null\ndomains:\n- domain: antavo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/security/antavo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Customer Loyalty
- Rewards
- Enterprise
- Headless
- Retail
- Marketing
- Engagement
- Promotions
- Gamification
- Events
- eCommerce
- Coupons
- Points
- Membership
---
