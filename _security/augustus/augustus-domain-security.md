---
api_specs:
- filename: augustus-account-programs-api-openapi.yml
  format: yaml
  label: Augustus Account Programs API
  slug: augustus-account-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-account-programs-api-openapi.yml
- filename: augustus-accounts-api-openapi.yml
  format: yaml
  label: Augustus Accounts API
  slug: augustus-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-accounts-api-openapi.yml
- filename: augustus-api-key-api-openapi.yml
  format: yaml
  label: Augustus API Key API
  slug: augustus-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-api-key-api-openapi.yml
- filename: augustus-api-versions-api-openapi.yml
  format: yaml
  label: Augustus API Versions API
  slug: augustus-api-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-api-versions-api-openapi.yml
- filename: augustus-conversions-api-openapi.yml
  format: yaml
  label: Augustus Conversions API
  slug: augustus-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-conversions-api-openapi.yml
- filename: augustus-deposits-api-openapi.yml
  format: yaml
  label: Augustus Deposits API
  slug: augustus-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-deposits-api-openapi.yml
- filename: augustus-events-api-openapi.yml
  format: yaml
  label: Augustus Events API
  slug: augustus-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-events-api-openapi.yml
- filename: augustus-payouts-api-openapi.yml
  format: yaml
  label: Augustus Payouts API
  slug: augustus-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-payouts-api-openapi.yml
- filename: augustus-quotes-api-openapi.yml
  format: yaml
  label: Augustus Quotes API
  slug: augustus-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-quotes-api-openapi.yml
- filename: augustus-returns-api-openapi.yml
  format: yaml
  label: Augustus Returns API
  slug: augustus-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-returns-api-openapi.yml
- filename: augustus-scopes-api-openapi.yml
  format: yaml
  label: Augustus Scopes API
  slug: augustus-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-scopes-api-openapi.yml
- filename: augustus-webhook-deliveries-api-openapi.yml
  format: yaml
  label: Augustus Webhook Deliveries API
  slug: augustus-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-webhook-deliveries-api-openapi.yml
- filename: augustus-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Augustus Webhook Subscriptions API
  slug: augustus-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/openapi/augustus-webhook-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: augustus.com
  spf: true
hosts:
- cert_expires: Oct  8 17:43:06 2026 GMT
  host: augustus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 09:25:51 2026 GMT
  host: docs.augustus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.augustus.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Augustus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augustus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Augustus
provider_slug: augustus
slug: augustus-domain-security
source_filename: augustus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: augustus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:43:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.augustus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:25:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.augustus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: augustus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augustus/refs/heads/main/security/augustus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Banking
- Open Banking
- Stablecoins
- Payouts
- Foreign Exchange
- Webhook
---
