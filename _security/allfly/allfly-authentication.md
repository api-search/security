---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allfly-connect-api-openapi.yml
  format: yaml
  label: AllFly Connect API
  slug: allfly-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allfly/refs/heads/main/openapi/allfly-connect-api-openapi.yml
- filename: allfly-events-api-openapi.yml
  format: yaml
  label: AllFly Events API
  slug: allfly-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allfly/refs/heads/main/openapi/allfly-events-api-openapi.yml
auth_types: []
description: Allfly Connect API uses API keys for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Allfly Authentication
name_suffix: Authentication
oauth_flows: []
overview: AllFly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AllFly
provider_slug: allfly
scheme_count: 1
schemes:
- evidence: API keys are required to authenticate requests to the Allfly Connect API.
  how_to_obtain: Create a new API key in the Integrations settings of your Allfly Quest account.
  name: API Key
  type: apiKey
slug: allfly-authentication
source_filename: allfly-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.allfly.io/api-key-management/
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.allfly.io/api-key-management/\nsources:\n- https://docs.allfly.io/api-key-management/\n- https://docs.allfly.io/api-key-management/\ndescription: Allfly Connect API uses API keys for authentication.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: API keys are required to authenticate requests to the Allfly Connect API.\n  how_to_obtain: Create a new API key in the Integrations settings of your Allfly Quest account.\ndocs: https://docs.allfly.io/api-key-management/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allfly/refs/heads/main/authentication/allfly-authentication.yml
summary_line: 1 scheme
tags:
- Travel
- CorporateTravel
- Marketplace
- Booking
- Software-as-a-Service
---
