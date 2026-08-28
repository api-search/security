---
api_specs:
- filename: mycarrier-public-api-openapi.json
  format: json
  label: MyCarrier Public API
  slug: mycarrier-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-public-api-openapi.json
- filename: mycarrier-order-public-api-openapi.json
  format: json
  label: MyCarrier Order API
  slug: mycarrier-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-order-public-api-openapi.json
- filename: mycarrier-freightaudit-api-openapi.json
  format: json
  label: MyCarrier FreightAudit API
  slug: mycarrier-freightaudit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-freightaudit-api-openapi.json
- filename: mycarrier-webhook-api-openapi.json
  format: json
  label: MyCarrier Webhook Registration API
  slug: mycarrier-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/openapi/mycarrier-webhook-api-openapi.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Mycarrier Trust Center
name_suffix: Trust Center
overview: MyCarrier maintains a public trust center covering its security and compliance posture.
provider_name: MyCarrier
provider_slug: mycarrier
slug: mycarrier-trust-center
source_filename: mycarrier-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.mycarrier.io/\npresent: true\nurl: https://trust.mycarrier.io/\nhttp_status: 200\nplatform: Vanta Trust Center\ncanonical: https://trust.mycarrier.io\nprogram_statement: 'MyCarrier is committed to maintaining a secure and compliant\n  environment, with controls continuously monitored and validated through our\n  Vanta-powered Trust Center.'\nprogram_statement_source: 'meta name=\"description\" on https://trust.mycarrier.io/'\ncertifications: []\ncertifications_note: 'MyCarrier operates a dedicated, live trust center on its own\n  subdomain, which is a published compliance program. The specific frameworks and audit\n  reports it lists could NOT be read: the page is a fully client-rendered Vanta\n  single-page application whose served HTML (5,750 bytes) contains only the document\n  shell, module preloads and Open Graph tags. Three candidate data endpoints\n  (/api/trust-center, /graphql, and the Vanta app path) each\
  \ returned the same SPA\n  shell rather than JSON. No named certification (SOC 2, ISO 27001, PCI DSS, HIPAA,\n  FedRAMP) is asserted here, because none was observed — recording one from inference\n  would be fabrication. Re-probe with a JS-capable fetch to enumerate the framework\n  list.'\ndocuments_gated: unknown\nnote: 'Most Vanta trust centers gate audit reports behind an NDA click-through; whether\n  MyCarrier does was not observable without rendering the page.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mycarrier/refs/heads/main/security/mycarrier-trust-center.yml
summary_line: trust center published
tags:
- Company
- Logistics
- Transportation
- Freight
- Shipping
- LTL
- Supply Chain
- Transportation Management
- Freight Audit
- Invoicing
trust_url: https://trust.mycarrier.io/
---
