---
anonymous_access: false
api_key_in: []
api_specs:
- filename: droplinked-com-openapi-generated.yml
  format: yaml
  label: Droplinked API
  slug: droplinked-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/droplinked-com/openapi/_ae-authored/droplinked-com-openapi-generated.yml
- filename: droplinked-com-openapi-openapi.json
  format: json
  label: Droplinked Openapi API
  slug: droplinked-openapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/droplinked-com/openapi/_original/droplinked-com-openapi-openapi.json
auth_types: []
description: Authentication schemes for Droplinked API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Droplinked Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Droplinked declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Droplinked
provider_slug: droplinked-com
scheme_count: 1
schemes:
- evidence: Partner/integration services authenticate to the Integration Services layer with an `integration-api-key` header.
  header: integration-api-key
  how_to_obtain: Issued by Droplinked as a partner integration key.
  location: header
  name: IntegrationKey
  type: apiKey
slug: droplinked-com-authentication
source_filename: droplinked-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.droplinked.com/authentication.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.droplinked.com/authentication.md\nsources:\n- https://docs.droplinked.com/authentication.md\n- https://docs.droplinked.com/api-reference/public/storefront-preview-token.md\n- https://docs.droplinked.com/api-reference/merchant/reset-merchant-password-with-reset-token.md\n- https://docs.droplinked.com/api-reference/merchant/refresh-access-token-using-refresh-token.md\ndescription: Authentication schemes for Droplinked API\nschemes:\n- type: apiKey\n  name: IntegrationKey\n  evidence: Partner/integration services authenticate to the Integration Services layer with an `integration-api-key` header.\n  location: header\n  header: integration-api-key\n  how_to_obtain: Issued by Droplinked as a partner integration key.\nnote: Public tier requires no authentication and is therefore not represented as a scheme. 2 extracted row(s) were dropped because their quote\n  was not on\
  \ the page.\ndocs: https://docs.droplinked.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/droplinked-com/authentication/droplinked-com-authentication.yml
summary_line: 1 scheme
tags:
- E-Commerce
- Artificial Intelligence
- catalog-import
- Online Store
- MCP
---
