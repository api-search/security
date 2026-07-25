---
api_specs:
- filename: aqueduct-accountowner-api-openapi.yml
  format: yaml
  label: Aqueduct AccountOwner API
  slug: aqueduct-accountowner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-accountowner-api-openapi.yml
- filename: aqueduct-bill-api-openapi.yml
  format: yaml
  label: Aqueduct Bill API
  slug: aqueduct-bill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-bill-api-openapi.yml
- filename: aqueduct-invoice-api-openapi.yml
  format: yaml
  label: Aqueduct Invoice API
  slug: aqueduct-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-invoice-api-openapi.yml
- filename: aqueduct-invoicelineitem-api-openapi.yml
  format: yaml
  label: Aqueduct InvoiceLineItem API
  slug: aqueduct-invoicelineitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-invoicelineitem-api-openapi.yml
- filename: aqueduct-pricemodel-api-openapi.yml
  format: yaml
  label: Aqueduct PriceModel API
  slug: aqueduct-pricemodel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-pricemodel-api-openapi.yml
- filename: aqueduct-productpurchases-api-openapi.yml
  format: yaml
  label: Aqueduct ProductPurchases API
  slug: aqueduct-productpurchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-productpurchases-api-openapi.yml
- filename: aqueduct-products-api-openapi.yml
  format: yaml
  label: Aqueduct Products API
  slug: aqueduct-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-products-api-openapi.yml
- filename: aqueduct-provisioning-api-openapi.yml
  format: yaml
  label: Aqueduct Provisioning API
  slug: aqueduct-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-provisioning-api-openapi.yml
- filename: aqueduct-subscriptions-api-openapi.yml
  format: yaml
  label: Aqueduct Subscriptions API
  slug: aqueduct-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-subscriptions-api-openapi.yml
- filename: aqueduct-webhooks-api-openapi.yml
  format: yaml
  label: Aqueduct Webhooks API
  slug: aqueduct-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/openapi/aqueduct-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tryaqueduct.com
  spf: true
hosts:
- host: www.tryaqueduct.com
  https: false
- host: api.tryaqueduct.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aqueduct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aqueduct, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Aqueduct
provider_slug: aqueduct
slug: aqueduct-domain-security
source_filename: aqueduct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryaqueduct.com\n  https: false\n- host: api.tryaqueduct.com\n  https: false\ndomains:\n- domain: tryaqueduct.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqueduct/refs/heads/main/security/aqueduct-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Fintech
- Billing
- Invoicing
- Metering
- Usage-Based
- Subscriptions
- Payments
- API
---
