---
api_specs:
- filename: grubhub-menu-openapi.yml
  format: yaml
  label: Grubhub Menu API
  slug: grubhub-menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-openapi.yml
- filename: grubhub-orders-openapi.yml
  format: yaml
  label: Grubhub Orders API
  slug: grubhub-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-openapi.yml
- filename: grubhub-merchant-data-openapi.yml
  format: yaml
  label: Grubhub Merchant Data API
  slug: grubhub-merchant-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-data-openapi.yml
- filename: grubhub-merchant-schedules-openapi.yml
  format: yaml
  label: Grubhub Merchant Schedules API
  slug: grubhub-merchant-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-schedules-openapi.yml
- filename: grubhub-busy-intervals-openapi.yml
  format: yaml
  label: Grubhub Busy Intervals API
  slug: grubhub-busy-intervals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-busy-intervals-openapi.yml
- filename: grubhub-deliveries-openapi.yml
  format: yaml
  label: Grubhub Deliveries API
  slug: grubhub-deliveries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-deliveries-openapi.yml
- filename: grubhub-connect-endpoints-openapi.yml
  format: yaml
  label: Grubhub Connect (Delivery as a Service) API
  slug: grubhub-connect-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-connect-endpoints-openapi.yml
- filename: grubhub-connect-webhooks-openapi.yml
  format: yaml
  label: Grubhub Connect Webhooks
  slug: grubhub-connect-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-connect-webhooks-openapi.yml
- filename: grubhub-onboarding-openapi.yml
  format: yaml
  label: Grubhub Onboarding API
  slug: grubhub-onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-onboarding-openapi.yml
- filename: grubhub-reporting-endpoints-openapi.yml
  format: yaml
  label: Grubhub Merchant Reporting API
  slug: grubhub-reporting-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-reporting-endpoints-openapi.yml
- filename: grubhub-reporting-webhooks-openapi.yml
  format: yaml
  label: Grubhub Reporting Webhooks
  slug: grubhub-reporting-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-reporting-webhooks-openapi.yml
- filename: grubhub-testing-openapi.yml
  format: yaml
  label: Grubhub Testing API
  slug: grubhub-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-testing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grubhub.com
  spf: true
hosts:
- cert_expires: Nov 24 01:08:20 2026 GMT
  host: grubhub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 01:08:20 2026 GMT
  host: developer.grubhub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.grubhub.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Grubhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grubhub, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Grubhub
provider_slug: grubhub
slug: grubhub-domain-security
source_filename: grubhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grubhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 01:08:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.grubhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 01:08:20 2026 GMT\n  hsts: false\n- host: api.grubhub.com\n  https: false\ndomains:\n- domain: grubhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/security/grubhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Delivery
- Restaurant
- Marketplace
- Online Ordering
- Point-of-Sale
- Logistics
- Last Mile Delivery
- Menu Management
- Hospitality
- Local Commerce
---
