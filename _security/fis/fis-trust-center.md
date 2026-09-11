---
api_specs:
- filename: fis-accounts-api-openapi.yml
  format: yaml
  label: FIS Global Accounts API
  slug: fis-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-accounts-api-openapi.yml
- filename: fis-ach-api-openapi.yml
  format: yaml
  label: FIS Global ACH API
  slug: fis-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-ach-api-openapi.yml
- filename: fis-payments-api-openapi.yml
  format: yaml
  label: FIS Global Payments API
  slug: fis-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-payments-api-openapi.yml
- filename: fis-transactions-api-openapi.yml
  format: yaml
  label: FIS Global Transactions API
  slug: fis-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-transactions-api-openapi.yml
- filename: fis-wire-transfers-api-openapi.yml
  format: yaml
  label: FIS Global Wire Transfers API
  slug: fis-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-wire-transfers-api-openapi.yml
- filename: fis-accounting-data-as-a-service-openapi.json
  format: json
  label: FIS Accounting Data as a Service
  slug: fis-accounting-data-as-a-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/_original/fis-accounting-data-as-a-service-openapi.json
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Fis Trust Center
name_suffix: Trust Center
overview: FIS Global maintains a public trust center covering its security and compliance posture.
provider_name: FIS Global
provider_slug: fis
slug: fis-trust-center
source_filename: fis-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: DNS + HTTP probes of the conventional trust-center hosts and a search of fisglobal.com\ntrust_center:\n  exists: false\ncertifications: []\nnote: >-\n  No public FIS trust center was found. trust.fisglobal.com, security.fisglobal.com and\n  status.fisglobal.com all return NXDOMAIN, and no certification index (SOC 2 / ISO 27001 /\n  PCI DSS attestation listing) is published on a page a member of the public can reach without\n  a customer login. FIS publishes compliance material inside client and RFP channels rather\n  than on an open trust page, so this is a recorded absence of a PUBLIC surface, not a claim\n  that FIS holds no certifications. No Compliance pointer is emitted, because there is no\n  published compliance program page to point at.\nevidence:\n- url: https://trust.fisglobal.com\n  status: 0\n  detail: NXDOMAIN\n- url: https://security.fisglobal.com\n  status: 0\n  detail: NXDOMAIN\n- url: https://status.fisglobal.com\n\
  \  status: 0\n  detail: NXDOMAIN\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/security/fis-trust-center.yml
summary_line: trust center published
tags:
- Banking
- Core Banking
- Financial-Services
- Payments
- Fintech
trust_url: ''
---
