---
api_specs:
- filename: punchh-mobile-api-openapi.yml
  format: yaml
  label: Punchh Mobile API
  slug: punchh-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-api-openapi.yml
- filename: punchh-mobile-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - Mobile
  slug: punchh-mobile-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-redemptions-legacy-openapi.yml
- filename: punchh-mobile-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - Mobile
  slug: punchh-mobile-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-redemptions-v2-openapi.yml
- filename: punchh-mobile-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Mobile
  slug: punchh-mobile-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-subscription-openapi.yml
- filename: punchh-online-ordering-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - Online Ordering
  slug: punchh-online-ordering-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-redemptions-legacy-openapi.yml
- filename: punchh-online-ordering-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - Online Ordering
  slug: punchh-online-ordering-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-redemptions-v2-openapi.yml
- filename: punchh-online-ordering-sso-api-openapi.yml
  format: yaml
  label: Punchh Online Ordering and SSO API
  slug: punchh-online-ordering-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-sso-api-openapi.yml
- filename: punchh-online-ordering-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Online Ordering
  slug: punchh-online-ordering-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-subscription-openapi.yml
- filename: punchh-platform-functions-api-openapi.yml
  format: yaml
  label: Punchh Platform Functions API
  slug: punchh-platform-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-api-openapi.yml
- filename: punchh-platform-functions-headless-offers-openapi.yml
  format: yaml
  label: Punchh Headless Offers API - Platform Functions
  slug: punchh-platform-functions-headless-offers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-headless-offers-openapi.yml
- filename: punchh-platform-functions-offers-ingestion-openapi.yml
  format: yaml
  label: Punchh Offers Ingestion API - Platform Functions
  slug: punchh-platform-functions-offers-ingestion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-offers-ingestion-openapi.yml
- filename: punchh-platform-functions-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Platform Functions
  slug: punchh-platform-functions-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-subscription-openapi.yml
- filename: punchh-pos-api-openapi.yml
  format: yaml
  label: Punchh POS API
  slug: punchh-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-api-openapi.yml
- filename: punchh-pos-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - POS
  slug: punchh-pos-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-redemptions-legacy-openapi.yml
- filename: punchh-pos-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - POS
  slug: punchh-pos-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-redemptions-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: punchh.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: partech.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: punchh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:18:33 2026 GMT
  host: developers.partech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Punchh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Punchh, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Punchh
provider_slug: punchh
slug: punchh-domain-security
source_filename: punchh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: punchh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\n- host: developers.partech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:18:33 2026 GMT\n  hsts: false\ndomains:\n- domain: punchh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: partech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/security/punchh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gift Cards
- Guest Engagement
- Loyalty
- Marketing
- Mobile
- Offers
- Online Ordering
- PAR Technology
- Point Of Sale
- Restaurant
- Restaurant Technology
- Webhooks
---
