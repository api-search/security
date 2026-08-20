---
api_specs:
- filename: talon-one-integration-api-openapi.yml
  format: yaml
  label: Talon.One Integration API
  slug: talon-one-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-integration-api-openapi.yml
- filename: talon-one-management-api-openapi.yml
  format: yaml
  label: Talon.One Management API
  slug: talon-one-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-management-api-openapi.yml
- filename: talon-one-third-party-api-openapi.yml
  format: yaml
  label: Talon.One Third-party API
  slug: talon-one-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-third-party-api-openapi.yml
- filename: talon-one-shopify-integration-api-openapi.yml
  format: yaml
  label: Talon.One Shopify Integration API
  slug: talon-one-shopify-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-shopify-integration-api-openapi.yml
- filename: talon-one-outbound-notifications-openapi.yml
  format: yaml
  label: Talon.One Outbound Notifications
  slug: talon-one-outbound-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-outbound-notifications-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: talon.one
  spf: true
hosts:
- cert_expires: Nov  9 16:26:54 2026 GMT
  host: www.talon.one
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 07:01:42 2026 GMT
  host: docs.talon.one
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 10:12:54 2026 GMT
  host: yourbaseurl.talon.one
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talon One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talon.One, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Talon.One
provider_slug: talon-one
slug: talon-one-domain-security
source_filename: talon-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.talon.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 16:26:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.talon.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:01:42 2026 GMT\n  hsts: false\n- host: yourbaseurl.talon.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:12:54 2026 GMT\n  hsts: null\ndomains:\n- domain: talon.one\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/security/talon-one-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Promotions
- Loyalty
- Coupons
- Incentives
- Campaigns
- Personalization
- MarTech
- Rules Engine
- Referrals
- Discounts
- E-Commerce
- Retail
---
