---
api_specs:
- filename: tamara-captures-api-openapi.yml
  format: yaml
  label: Tamara Captures API
  slug: tamara-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-captures-api-openapi.yml
- filename: tamara-channel-partner-webhooks-api-openapi.yml
  format: yaml
  label: Tamara Channel Partner Webhooks API
  slug: tamara-channel-partner-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-channel-partner-webhooks-api-openapi.yml
- filename: tamara-checkout-sessions-api-openapi.yml
  format: yaml
  label: Tamara Checkout Sessions API
  slug: tamara-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-checkout-sessions-api-openapi.yml
- filename: tamara-merchant-api-keys-api-openapi.yml
  format: yaml
  label: Tamara Merchant API Keys API
  slug: tamara-merchant-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-merchant-api-keys-api-openapi.yml
- filename: tamara-merchant-onboarding-api-openapi.yml
  format: yaml
  label: Tamara Merchant Onboarding API
  slug: tamara-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-merchant-onboarding-api-openapi.yml
- filename: tamara-refunds-api-openapi.yml
  format: yaml
  label: Tamara Refunds API
  slug: tamara-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/openapi/tamara-refunds-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tamara.co
  spf: true
hosts:
- cert_expires: Sep 17 04:03:10 2026 GMT
  host: docs.tamara.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 07:18:34 2027 GMT
  host: api.tamara.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 07:18:34 2027 GMT
  host: partner-api.tamara.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tamara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tamara, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tamara
provider_slug: tamara
slug: tamara-domain-security
source_filename: tamara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.tamara.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 04:03:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tamara.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 07:18:34 2027 GMT\n  hsts: null\n- host: partner-api.tamara.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 07:18:34 2027 GMT\n  hsts: null\ndomains:\n- domain: tamara.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/security/tamara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- BNPL
- Buy Now Pay Later
- Fintech
- Payments
- Checkout
- Shariah Compliant
- MENA
- Saudi Arabia
- UAE
- Installments
- Pay Later
- Merchant Services
- Order
- Refunds
- Capture
- Webhook
- Disputes
- Channel Partners
- E-Commerce
- Point-of-Sale
---
