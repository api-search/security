---
api_specs:
- filename: ometria-contacts-api-openapi.yml
  format: yaml
  label: Ometria Contacts API
  slug: ometria-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-contacts-api-openapi.yml
- filename: ometria-custom-event-api-openapi.yml
  format: yaml
  label: Ometria Custom Event API
  slug: ometria-custom-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-custom-event-api-openapi.yml
- filename: ometria-custom-fields-api-openapi.yml
  format: yaml
  label: Ometria Custom Fields API
  slug: ometria-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-custom-fields-api-openapi.yml
- filename: ometria-field-forget-email-phone-erasure-api-openapi.yml
  format: yaml
  label: Ometria Field forget (email / phone erasure) API
  slug: ometria-field-forget-email-phone-erasure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-field-forget-email-phone-erasure-api-openapi.yml
- filename: ometria-gdpr-anonymisation-requests-api-openapi.yml
  format: yaml
  label: Ometria GDPR anonymisation requests API
  slug: ometria-gdpr-anonymisation-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-gdpr-anonymisation-requests-api-openapi.yml
- filename: ometria-lists-api-openapi.yml
  format: yaml
  label: Ometria Lists API
  slug: ometria-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-lists-api-openapi.yml
- filename: ometria-orders-api-openapi.yml
  format: yaml
  label: Ometria Orders API
  slug: ometria-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-orders-api-openapi.yml
- filename: ometria-products-api-openapi.yml
  format: yaml
  label: Ometria Products API
  slug: ometria-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-products-api-openapi.yml
- filename: ometria-profiles-api-openapi.yml
  format: yaml
  label: Ometria Profiles API
  slug: ometria-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-profiles-api-openapi.yml
- filename: ometria-push-api-openapi.yml
  format: yaml
  label: Ometria Push API
  slug: ometria-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-push-api-openapi.yml
- filename: ometria-transactional-email-api-openapi.yml
  format: yaml
  label: Ometria Transactional Email API
  slug: ometria-transactional-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-transactional-email-api-openapi.yml
- filename: ometria-translation-requests-api-openapi.yml
  format: yaml
  label: Ometria Translation Requests API
  slug: ometria-translation-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-translation-requests-api-openapi.yml
- filename: ometria-unsubscribes-api-openapi.yml
  format: yaml
  label: Ometria Unsubscribes API
  slug: ometria-unsubscribes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-unsubscribes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ometria.com
  spf: true
hosts:
- cert_expires: Dec 30 10:17:29 2026 GMT
  host: ometria.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ometria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ometria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ometria
provider_slug: ometria
slug: ometria-domain-security
source_filename: ometria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ometria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 10:17:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ometria.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ometria/security/ometria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Customer Data Platform
- AI
- Marketing
---
