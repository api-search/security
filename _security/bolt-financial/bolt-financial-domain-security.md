---
api_specs:
- filename: bolt-financial-account-api-openapi.yml
  format: yaml
  label: Bolt Financial Account API
  slug: bolt-financial-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-account-api-openapi.yml
- filename: bolt-financial-callbacks-api-openapi.yml
  format: yaml
  label: Bolt Financial Callbacks API
  slug: bolt-financial-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-callbacks-api-openapi.yml
- filename: bolt-financial-configuration-api-openapi.yml
  format: yaml
  label: Bolt Financial Configuration API
  slug: bolt-financial-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-configuration-api-openapi.yml
- filename: bolt-financial-oauth-api-openapi.yml
  format: yaml
  label: Bolt Financial O Auth API
  slug: bolt-financial-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-oauth-api-openapi.yml
- filename: bolt-financial-orders-api-openapi.yml
  format: yaml
  label: Bolt Financial Orders API
  slug: bolt-financial-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-orders-api-openapi.yml
- filename: bolt-financial-payments-api-openapi.yml
  format: yaml
  label: Bolt Financial Payments API
  slug: bolt-financial-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-payments-api-openapi.yml
- filename: bolt-financial-statements-api-openapi.yml
  format: yaml
  label: Bolt Financial Statements API
  slug: bolt-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-statements-api-openapi.yml
- filename: bolt-financial-subscriptions-api-openapi.yml
  format: yaml
  label: Bolt Financial Subscriptions API
  slug: bolt-financial-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-subscriptions-api-openapi.yml
- filename: bolt-financial-testing-api-openapi.yml
  format: yaml
  label: Bolt Financial Testing API
  slug: bolt-financial-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-testing-api-openapi.yml
- filename: bolt-financial-tokenizer-api-openapi.yml
  format: yaml
  label: Bolt Financial Tokenizer API
  slug: bolt-financial-tokenizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-tokenizer-api-openapi.yml
- filename: bolt-financial-transactions-api-openapi.yml
  format: yaml
  label: Bolt Financial Transactions API
  slug: bolt-financial-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-transactions-api-openapi.yml
- filename: bolt-financial-webhooks-api-openapi.yml
  format: yaml
  label: Bolt Financial Webhooks API
  slug: bolt-financial-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/openapi/bolt-financial-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bolt.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boltapp.com
  spf: true
hosts:
- cert_expires: Oct 12 14:53:16 2026 GMT
  host: www.bolt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 18:22:53 2026 GMT
  host: help.boltapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.boltapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bolt Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolt Financial, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bolt Financial
provider_slug: bolt-financial
slug: bolt-financial-domain-security
source_filename: bolt-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bolt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 14:53:16 2026 GMT\n  hsts: null\n- host: help.boltapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 18:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.boltapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bolt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: boltapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-financial/refs/heads/main/security/bolt-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Checkout
- E-Commerce
- Fintech
- Subscription
- Tokenization
- Fraud
- Identity
- Webhook
---
