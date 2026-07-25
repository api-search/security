---
api_specs:
- filename: talon-one-account-api-openapi.yml
  format: yaml
  label: Talon.One Account API
  slug: talon-one-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-account-api-openapi.yml
- filename: talon-one-applications-api-openapi.yml
  format: yaml
  label: Talon.One Applications API
  slug: talon-one-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-applications-api-openapi.yml
- filename: talon-one-attributes-api-openapi.yml
  format: yaml
  label: Talon.One Attributes API
  slug: talon-one-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-attributes-api-openapi.yml
- filename: talon-one-audiences-api-openapi.yml
  format: yaml
  label: Talon.One Audiences API
  slug: talon-one-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-audiences-api-openapi.yml
- filename: talon-one-campaigns-api-openapi.yml
  format: yaml
  label: Talon.One Campaigns API
  slug: talon-one-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-campaigns-api-openapi.yml
- filename: talon-one-collections-api-openapi.yml
  format: yaml
  label: Talon.One Collections API
  slug: talon-one-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-collections-api-openapi.yml
- filename: talon-one-coupons-api-openapi.yml
  format: yaml
  label: Talon.One Coupons API
  slug: talon-one-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-coupons-api-openapi.yml
- filename: talon-one-customer-profiles-api-openapi.yml
  format: yaml
  label: Talon.One Customer Profiles API
  slug: talon-one-customer-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-customer-profiles-api-openapi.yml
- filename: talon-one-customer-sessions-api-openapi.yml
  format: yaml
  label: Talon.One Customer Sessions API
  slug: talon-one-customer-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-customer-sessions-api-openapi.yml
- filename: talon-one-events-api-openapi.yml
  format: yaml
  label: Talon.One Events API
  slug: talon-one-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-events-api-openapi.yml
- filename: talon-one-exports-api-openapi.yml
  format: yaml
  label: Talon.One Exports API
  slug: talon-one-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-exports-api-openapi.yml
- filename: talon-one-loyalty-api-openapi.yml
  format: yaml
  label: Talon.One Loyalty API
  slug: talon-one-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-loyalty-api-openapi.yml
- filename: talon-one-referrals-api-openapi.yml
  format: yaml
  label: Talon.One Referrals API
  slug: talon-one-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-referrals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: talon.one
  spf: true
hosts:
- cert_expires: Sep  8 21:09:10 2026 GMT
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
- cert_expires: Sep 16 07:01:42 2026 GMT
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
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.talon.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:09:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.talon.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:01:42 2026 GMT\n  hsts: false\n- host: yourbaseurl.talon.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:01:42 2026 GMT\n  hsts: null\ndomains:\n- domain: talon.one\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
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
---
