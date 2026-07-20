---
api_specs:
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Accept API (Singapore)
  slug: fazz-accept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Send API (Singapore)
  slug: fazz-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Payment Methods API
  slug: fazz-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Fazz Trust Center
name_suffix: Trust Center
overview: Fazz maintains a public trust center covering its security and compliance posture.
provider_name: Fazz
provider_slug: fazz
slug: fazz-trust-center
source_filename: fazz-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nprobe: true\nsource: https://fazz.com/ ; https://docs.fazz.com/\nurl: https://fazz.com/\ncertifications: []\nregulatory:\n- authority: Monetary Authority of Singapore (MAS)\n  note: >-\n    Fazz Business Singapore operates through Xfers Pte. Ltd., which is\n    regulated under Singapore's Payment Services Act. Confirm current\n    Major Payment Institution licence status on the MAS Financial\n    Institutions Directory during reconciliation.\n  confidence: reported-unverified\n- authority: Bank Indonesia / OJK\n  note: >-\n    Fazz's Indonesia operations (formerly Payfazz / PT) are subject to\n    Bank Indonesia and OJK payment regulation. Verify specific licences\n    during reconciliation.\n  confidence: reported-unverified\nevidence:\n- source: https://fazz.com/business/products/payments-api/\n  note: >-\n    Product page markets \"send and receive payments securely\" but does not\n    enumerate PCI DSS / ISO 27001 / SOC 2 certifications.\n\
  - source: probe\n  note: >-\n    No /.well-known/security.txt found on fazz.com or www.xfers.io (HTTP 404),\n    and no dedicated public trust-center / compliance page was located via\n    search as of the generated date.\nnotes: >-\n  No first-party trust center enumerating security certifications was found.\n  Regulatory posture is recorded as reported-unverified pending confirmation\n  against MAS / Bank Indonesia / OJK registries. Do not represent\n  certifications that are not published by the provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/security/fazz-trust-center.yml
summary_line: trust center published
tags:
- Fintech
- Payments
- Business Banking
- Disbursements
- Southeast Asia
- PayNow
- Virtual Accounts
trust_url: https://fazz.com/
---
