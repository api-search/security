---
api_specs:
- filename: rye-betas-api-openapi.yml
  format: yaml
  label: Rye Betas API
  slug: rye-betas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-betas-api-openapi.yml
- filename: rye-billing-api-openapi.yml
  format: yaml
  label: Rye Billing API
  slug: rye-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-billing-api-openapi.yml
- filename: rye-brands-api-openapi.yml
  format: yaml
  label: Rye Brands API
  slug: rye-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-brands-api-openapi.yml
- filename: rye-checkout-intents-api-openapi.yml
  format: yaml
  label: Rye Checkout Intents API
  slug: rye-checkout-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-checkout-intents-api-openapi.yml
- filename: rye-commissions-api-openapi.yml
  format: yaml
  label: Rye Commissions API
  slug: rye-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-commissions-api-openapi.yml
- filename: rye-events-api-openapi.yml
  format: yaml
  label: Rye Events API
  slug: rye-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-events-api-openapi.yml
- filename: rye-merchant-connectors-api-openapi.yml
  format: yaml
  label: Rye Merchant Connectors API
  slug: rye-merchant-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-merchant-connectors-api-openapi.yml
- filename: rye-orders-api-openapi.yml
  format: yaml
  label: Rye Orders API
  slug: rye-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-orders-api-openapi.yml
- filename: rye-payment-gateways-api-openapi.yml
  format: yaml
  label: Rye Payment Gateways API
  slug: rye-payment-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-payment-gateways-api-openapi.yml
- filename: rye-products-api-openapi.yml
  format: yaml
  label: Rye Products API
  slug: rye-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-products-api-openapi.yml
- filename: rye-returns-api-openapi.yml
  format: yaml
  label: Rye Returns API
  slug: rye-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-returns-api-openapi.yml
- filename: rye-shipments-api-openapi.yml
  format: yaml
  label: Rye Shipments API
  slug: rye-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-shipments-api-openapi.yml
- filename: rye-test-helpers-api-openapi.yml
  format: yaml
  label: Rye Test Helpers API
  slug: rye-test-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/openapi/rye-test-helpers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rye.com
  spf: true
hosts:
- cert_expires: Sep 20 08:38:52 2026 GMT
  host: staging.api.rye.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rye
provider_slug: rye
slug: rye-domain-security
source_filename: rye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: staging.api.rye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:38:52 2026 GMT\n  hsts: null\ndomains:\n- domain: rye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rye/refs/heads/main/security/rye-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Checkout
- Payments
- Agentic Commerce
- AI Agents
- Universal Checkout
- Shopping
---
