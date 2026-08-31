---
api_specs:
- filename: imprint-customer-links-api-openapi.yml
  format: yaml
  label: Imprint Customer Links API
  slug: imprint-customer-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-customer-links-api-openapi.yml
- filename: imprint-customer-sessions-api-openapi.yml
  format: yaml
  label: Imprint Customer Sessions API
  slug: imprint-customer-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-customer-sessions-api-openapi.yml
- filename: imprint-customers-api-openapi.yml
  format: yaml
  label: Imprint Customers API
  slug: imprint-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-customers-api-openapi.yml
- filename: imprint-keys-api-openapi.yml
  format: yaml
  label: Imprint Keys API
  slug: imprint-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-keys-api-openapi.yml
- filename: imprint-offers-api-openapi.yml
  format: yaml
  label: Imprint Offers API
  slug: imprint-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-offers-api-openapi.yml
- filename: imprint-order-events-api-openapi.yml
  format: yaml
  label: Imprint Order Events API
  slug: imprint-order-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-order-events-api-openapi.yml
- filename: imprint-orders-api-openapi.yml
  format: yaml
  label: Imprint Orders API
  slug: imprint-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-orders-api-openapi.yml
- filename: imprint-payment-methods-api-openapi.yml
  format: yaml
  label: Imprint Payment Methods API
  slug: imprint-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-payment-methods-api-openapi.yml
- filename: imprint-rewards-api-openapi.yml
  format: yaml
  label: Imprint Rewards API
  slug: imprint-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-rewards-api-openapi.yml
- filename: imprint-simulate-reward-api-openapi.yml
  format: yaml
  label: Imprint Simulate Reward API
  slug: imprint-simulate-reward-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-simulate-reward-api-openapi.yml
- filename: imprint-simulate-statement-reward-api-openapi.yml
  format: yaml
  label: Imprint Simulate Statement Reward API
  slug: imprint-simulate-statement-reward-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-simulate-statement-reward-api-openapi.yml
- filename: imprint-simulate-transaction-event-api-openapi.yml
  format: yaml
  label: Imprint Simulate Transaction Event API
  slug: imprint-simulate-transaction-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-simulate-transaction-event-api-openapi.yml
- filename: imprint-transaction-intents-api-openapi.yml
  format: yaml
  label: Imprint Transaction Intents API
  slug: imprint-transaction-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-transaction-intents-api-openapi.yml
- filename: imprint-transactions-api-openapi.yml
  format: yaml
  label: Imprint Transactions API
  slug: imprint-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-transactions-api-openapi.yml
- filename: imprint-webhooks-api-openapi.yml
  format: yaml
  label: Imprint Webhooks API
  slug: imprint-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: imprint.co
  spf: true
hosts:
- cert_expires: Oct  8 22:44:49 2026 GMT
  host: imprint.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 17:05:19 2026 GMT
  host: dev.sbx.imprint.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imprint, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Imprint
provider_slug: imprint
slug: imprint-domain-security
source_filename: imprint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imprint.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:44:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.sbx.imprint.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:05:19 2026 GMT\n  hsts: null\ndomains:\n- domain: imprint.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/security/imprint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial-Services
- Fintech
- Credit Cards
- Co-Branded Cards
- Payments
- Loans
- Rewards
- Loyalty
- Embedded Finance
---
