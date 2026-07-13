---
api_specs:
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Customers API
  slug: loyaltylion-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Activities API
  slug: loyaltylion-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Points API
  slug: loyaltylion-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Rewards API
  slug: loyaltylion-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Redemptions API
  slug: loyaltylion-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loyaltylion.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: loyaltylion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 10:29:08 2026 GMT
  host: developers.loyaltylion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: api.loyaltylion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loyaltylion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LoyaltyLion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LoyaltyLion
provider_slug: loyaltylion
slug: loyaltylion-domain-security
source_filename: loyaltylion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loyaltylion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\n- host: developers.loyaltylion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:29:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.loyaltylion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: loyaltylion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/security/loyaltylion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Rewards
- E-commerce
- Points
- Shopify
- Retention
---
