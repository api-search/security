---
api_specs:
- filename: overflow-campaigns-api-openapi.yml
  format: yaml
  label: Overflow Campaigns API
  slug: overflow-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-campaigns-api-openapi.yml
- filename: overflow-chargebacks-api-openapi.yml
  format: yaml
  label: Overflow Chargebacks API
  slug: overflow-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-chargebacks-api-openapi.yml
- filename: overflow-contributions-api-openapi.yml
  format: yaml
  label: Overflow Contributions API
  slug: overflow-contributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-contributions-api-openapi.yml
- filename: overflow-deposits-api-openapi.yml
  format: yaml
  label: Overflow Deposits API
  slug: overflow-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-deposits-api-openapi.yml
- filename: overflow-donors-api-openapi.yml
  format: yaml
  label: Overflow Donors API
  slug: overflow-donors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-donors-api-openapi.yml
- filename: overflow-locations-api-openapi.yml
  format: yaml
  label: Overflow Locations API
  slug: overflow-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-locations-api-openapi.yml
- filename: overflow-payment-methods-api-openapi.yml
  format: yaml
  label: Overflow Payment Methods API
  slug: overflow-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-payment-methods-api-openapi.yml
- filename: overflow-payments-api-openapi.yml
  format: yaml
  label: Overflow Payments API
  slug: overflow-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-payments-api-openapi.yml
- filename: overflow-refunds-api-openapi.yml
  format: yaml
  label: Overflow Refunds API
  slug: overflow-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-refunds-api-openapi.yml
- filename: overflow-status-api-openapi.yml
  format: yaml
  label: Overflow Status API
  slug: overflow-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-status-api-openapi.yml
- filename: overflow-subscriptions-api-openapi.yml
  format: yaml
  label: Overflow Subscriptions API
  slug: overflow-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-subscriptions-api-openapi.yml
- filename: overflow-tap-api-openapi.yml
  format: yaml
  label: Overflow Tap API
  slug: overflow-tap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-tap-api-openapi.yml
- filename: overflow-webhooks-api-openapi.yml
  format: yaml
  label: Overflow Webhooks API
  slug: overflow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: overflow.co
  spf: true
hosts:
- cert_expires: Oct 10 20:49:22 2026 GMT
  host: docs.overflow.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: server.overflow.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: server.stage.overflow.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overflow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Overflow
provider_slug: overflow
slug: overflow-domain-security
source_filename: overflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.overflow.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 20:49:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: server.overflow.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\n- host: server.stage.overflow.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: overflow.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/security/overflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Donations
- Fundraising
- Nonprofit
- Giving
- Recurring Payments
- Webhooks
- Cryptocurrency
---
