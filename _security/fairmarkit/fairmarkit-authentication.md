---
api_key_in:
- header
api_specs:
- filename: fairmarkit-business-units-api-openapi.yml
  format: yaml
  label: Fairmarkit Business Units API
  slug: fairmarkit-business-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-business-units-api-openapi.yml
- filename: fairmarkit-categories-api-openapi.yml
  format: yaml
  label: Fairmarkit Categories API
  slug: fairmarkit-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-categories-api-openapi.yml
- filename: fairmarkit-data-exports-api-openapi.yml
  format: yaml
  label: Fairmarkit Data Exports API
  slug: fairmarkit-data-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-data-exports-api-openapi.yml
- filename: fairmarkit-data-fields-api-openapi.yml
  format: yaml
  label: Fairmarkit Data Fields API
  slug: fairmarkit-data-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-data-fields-api-openapi.yml
- filename: fairmarkit-erp-systems-api-openapi.yml
  format: yaml
  label: Fairmarkit ERP Systems API
  slug: fairmarkit-erp-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-erp-systems-api-openapi.yml
- filename: fairmarkit-event-api-openapi.yml
  format: yaml
  label: Fairmarkit Event API
  slug: fairmarkit-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-event-api-openapi.yml
- filename: fairmarkit-file-attachments-api-openapi.yml
  format: yaml
  label: Fairmarkit File attachments API
  slug: fairmarkit-file-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-file-attachments-api-openapi.yml
- filename: fairmarkit-identity-api-openapi.yml
  format: yaml
  label: Fairmarkit Identity API
  slug: fairmarkit-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-identity-api-openapi.yml
- filename: fairmarkit-price-books-api-openapi.yml
  format: yaml
  label: Fairmarkit Price Books API
  slug: fairmarkit-price-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-price-books-api-openapi.yml
- filename: fairmarkit-purchase-orders-api-openapi.yml
  format: yaml
  label: Fairmarkit Purchase Orders API
  slug: fairmarkit-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-purchase-orders-api-openapi.yml
- filename: fairmarkit-requests-api-openapi.yml
  format: yaml
  label: Fairmarkit Requests API
  slug: fairmarkit-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-requests-api-openapi.yml
- filename: fairmarkit-responses-api-openapi.yml
  format: yaml
  label: Fairmarkit Responses API
  slug: fairmarkit-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-responses-api-openapi.yml
- filename: fairmarkit-rfp-api-openapi.yml
  format: yaml
  label: Fairmarkit RFP API
  slug: fairmarkit-rfp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-rfp-api-openapi.yml
- filename: fairmarkit-rfq-api-openapi.yml
  format: yaml
  label: Fairmarkit RFQ API
  slug: fairmarkit-rfq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-rfq-api-openapi.yml
- filename: fairmarkit-schema-api-openapi.yml
  format: yaml
  label: Fairmarkit Schema API
  slug: fairmarkit-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-schema-api-openapi.yml
- filename: fairmarkit-supplier-api-openapi.yml
  format: yaml
  label: Fairmarkit Supplier API
  slug: fairmarkit-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-supplier-api-openapi.yml
- filename: fairmarkit-uom-api-openapi.yml
  format: yaml
  label: Fairmarkit UOM API
  slug: fairmarkit-uom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-uom-api-openapi.yml
- filename: fairmarkit-user-profiles-api-openapi.yml
  format: yaml
  label: Fairmarkit User Profiles API
  slug: fairmarkit-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-user-profiles-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fairmarkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fairmarkit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fairmarkit
provider_slug: fairmarkit
scheme_count: 1
schemes:
- applies_to:
  - openapi/fairmarkit-buyer-openapi.json
  - openapi/fairmarkit-supplier-openapi.json
  description: API key generated by a Buyer-Admin or Supplier-Admin in Administration / Fairmarkit API settings. Sent on every request in the X-FM-API-KEY header. Generating a new buyer key deactivates prior keys; suppliers may hold up to 5 keys.
  in: header
  name: ApiKeyAuth
  parameter: X-FM-API-KEY
  type: apiKey
slug: fairmarkit-authentication
source_filename: fairmarkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.fairmarkit.com/docs/authentication-guide\ndocs: https://developers.fairmarkit.com/docs/authentication-guide\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-FM-API-KEY\n  description: API key generated by a Buyer-Admin or Supplier-Admin in Administration / Fairmarkit API\n    settings. Sent on every request in the X-FM-API-KEY header. Generating a new buyer key deactivates\n    prior keys; suppliers may hold up to 5 keys.\n  applies_to:\n  - openapi/fairmarkit-buyer-openapi.json\n  - openapi/fairmarkit-supplier-openapi.json\nnote: The published OpenAPI documents do not declare a securityScheme; the API-key model is documented\n  in the developer portal auth guide and captured here + in overlays/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/authentication/fairmarkit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Procurement
- Sourcing
- Supply Chain
- Purchasing
- Suppliers
- RFQ
- RFP
- Spend Management
- Webhooks
---
