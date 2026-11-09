---
anonymous_access: false
api_key_in: []
api_specs:
- filename: attestwire-com-billing-api-openapi.yml
  format: yaml
  label: Attestwire Billing API
  slug: attestwire-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-billing-api-openapi.yml
- filename: attestwire-com-diagnose-api-openapi.yml
  format: yaml
  label: Attestwire Diagnose API
  slug: attestwire-com-diagnose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-diagnose-api-openapi.yml
- filename: attestwire-com-invoices-api-openapi.yml
  format: yaml
  label: Attestwire Invoices API
  slug: attestwire-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-invoices-api-openapi.yml
- filename: attestwire-com-keys-api-openapi.yml
  format: yaml
  label: Attestwire Keys API
  slug: attestwire-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-keys-api-openapi.yml
- filename: attestwire-com-meta-api-openapi.yml
  format: yaml
  label: Attestwire Meta API
  slug: attestwire-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-meta-api-openapi.yml
- filename: attestwire-com-peppol-api-openapi.yml
  format: yaml
  label: Attestwire Peppol API
  slug: attestwire-com-peppol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-peppol-api-openapi.yml
- filename: attestwire-com-recipient-api-openapi.yml
  format: yaml
  label: Attestwire Recipient API
  slug: attestwire-com-recipient-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-recipient-api-openapi.yml
- filename: attestwire-com-records-api-openapi.yml
  format: yaml
  label: Attestwire Records API
  slug: attestwire-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-records-api-openapi.yml
- filename: attestwire-com-vat-api-openapi.yml
  format: yaml
  label: Attestwire Vat API
  slug: attestwire-com-vat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-vat-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Attestwire Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Attestwire declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Attestwire
provider_slug: attestwire-com
scheme_count: 1
schemes:
- description: A bearer token on every metered endpoint. Keys look like aw_live_ followed by 40 characters. Public demo key 'demo' works for limited endpoints.
  scheme: bearer
  type: http
slug: attestwire-com-authentication
source_filename: attestwire-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://api.attestwire.com/docs#auth\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"A bearer token on every metered endpoint. Keys look like aw_live_ followed by 40 characters. Public demo key 'demo' works for limited endpoints.\"\n"
source_yaml_url: https://artifacts.apis.io/attestwire-com/authentication/attestwire-com-authentication.yml
summary_line: 1 scheme
tags:
- Attestwire
- E-invoice
- Validation
- XRechnung
- PEPPOL
- MCP
---
