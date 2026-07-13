---
api_specs:
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Subscribers API
  slug: revenuecat-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Purchases & Receipts API
  slug: revenuecat-purchases-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Entitlements API (v1)
  slug: revenuecat-entitlements-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Offerings API (v1)
  slug: revenuecat-offerings-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Customer Attributes API
  slug: revenuecat-customer-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Projects API (v2)
  slug: revenuecat-projects-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Apps API (v2)
  slug: revenuecat-apps-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Customers API (v2)
  slug: revenuecat-customers-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Products API (v2)
  slug: revenuecat-products-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Entitlements API (v2)
  slug: revenuecat-entitlements-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Offerings API (v2)
  slug: revenuecat-offerings-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Packages API (v2)
  slug: revenuecat-packages-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: revenuecat.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.revenuecat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.revenuecat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revenuecat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RevenueCat, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RevenueCat
provider_slug: revenuecat
slug: revenuecat-domain-security
source_filename: revenuecat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revenuecat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.revenuecat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: revenuecat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/security/revenuecat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Subscriptions
- In-App Purchases
- Billing
- Mobile
- Entitlements
---
