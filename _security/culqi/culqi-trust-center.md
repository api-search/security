---
api_specs:
- filename: culqi-3ds-api-openapi.yml
  format: yaml
  label: Culqi 3DS API
  slug: culqi-3ds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-3ds-api-openapi.yml
- filename: culqi-cards-api-openapi.yml
  format: yaml
  label: Culqi Cards API
  slug: culqi-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-cards-api-openapi.yml
- filename: culqi-charges-api-openapi.yml
  format: yaml
  label: Culqi Charges API
  slug: culqi-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-charges-api-openapi.yml
- filename: culqi-customers-api-openapi.yml
  format: yaml
  label: Culqi Customers API
  slug: culqi-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-customers-api-openapi.yml
- filename: culqi-events-api-openapi.yml
  format: yaml
  label: Culqi Events API
  slug: culqi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-events-api-openapi.yml
- filename: culqi-iins-api-openapi.yml
  format: yaml
  label: Culqi Iins API
  slug: culqi-iins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-iins-api-openapi.yml
- filename: culqi-orders-api-openapi.yml
  format: yaml
  label: Culqi Orders API
  slug: culqi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-orders-api-openapi.yml
- filename: culqi-plans-api-openapi.yml
  format: yaml
  label: Culqi Plans API
  slug: culqi-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-plans-api-openapi.yml
- filename: culqi-refunds-api-openapi.yml
  format: yaml
  label: Culqi Refunds API
  slug: culqi-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-refunds-api-openapi.yml
- filename: culqi-subscriptions-api-openapi.yml
  format: yaml
  label: Culqi Subscriptions API
  slug: culqi-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-subscriptions-api-openapi.yml
- filename: culqi-tokens-api-openapi.yml
  format: yaml
  label: Culqi Tokens API
  slug: culqi-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-tokens-api-openapi.yml
- filename: culqi-transfers-api-openapi.yml
  format: yaml
  label: Culqi Transfers API
  slug: culqi-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/openapi/culqi-transfers-api-openapi.yml
certifications:
- PCI DSS Level 1
description: ''
kind: trust-center
layout: security
name: Culqi Trust Center
name_suffix: Trust Center
overview: Culqi maintains a public trust center documenting PCI DSS Level 1 compliance.
provider_name: Culqi
provider_slug: culqi
slug: culqi-trust-center
source_filename: culqi-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nprobe: true\nsource: https://docs.culqi.com/ + https://culqi.com/\ncertifications:\n- PCI DSS Level 1\nevidence:\n- source: https://docs.culqi.com/\n  keywords:\n  - pci dss\n  - pci dss 3.2\n  - saq-d\n  - tokenizacion\n  - 3ds\n  - antifraude\n- source: https://culqi.com/\n  keywords:\n  - pci dss\n  - seguridad\nnotes: >-\n  Culqi is a PCI DSS Level 1 compliant payment processor; card data is\n  tokenized client-side (Culqi Checkout / Culqi JS v4) so raw card numbers do\n  not touch merchant servers. Merchants that call the API directly with raw\n  card data must themselves comply with PCI DSS 3.2 and submit an SAQ-D.\n  Culqi provides 3-D Secure (Culqi 3DS) and antifraud (antifraude) device\n  fingerprinting for card-not-present risk control. As a Grupo Credicorp /\n  Krealo company, Culqi operates under Peru's financial-sector regulatory\n  regime (SBS). No standalone public trust-center portal (e.g. a Vanta/Drata\n  trust page)\
  \ was located at probe time; compliance is documented within the\n  developer docs and corporate site.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culqi/refs/heads/main/security/culqi-trust-center.yml
summary_line: PCI DSS Level 1
tags:
- Payments
- Payment Gateway
- FinTech
- Peru
- LatAm
- Cards
- Yape
trust_url: ''
---
