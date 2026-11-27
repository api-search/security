---
anonymous_access: false
api_key_in: []
api_specs:
- filename: easyemailverification-com-account-api-openapi.yml
  format: yaml
  label: Easy Email Verification Account API
  slug: easyemailverification-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-account-api-openapi.yml
- filename: easyemailverification-com-bulk-verification-api-openapi.yml
  format: yaml
  label: Easy Email Verification Bulk Verification API
  slug: easyemailverification-com-bulk-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-bulk-verification-api-openapi.yml
- filename: easyemailverification-com-single-verification-api-openapi.yml
  format: yaml
  label: Easy Email Verification Single Verification API
  slug: easyemailverification-com-single-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-single-verification-api-openapi.yml
auth_types: []
description: Easy Email Verification authenticates API requests using an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Easy Email Verification Authentication
name_suffix: Authentication
oauth_flows: []
overview: Easy Email Verification declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Easy Email Verification
provider_slug: easyemailverification-com
scheme_count: 1
schemes:
- evidence: Send the key in the `X-API-Key` header (recommended). The `apikey` query parameter and the `Authorization` header also work; see the API reference.
  header: X-API-Key
  how_to_obtain: Create an account at https://dashboard.easyemailverification.com/register and generate an API key at https://dashboard.easyemailverification.com/apisettings.
  location: header
  name: X-API-Key
  type: apiKey
slug: easyemailverification-com-authentication
source_filename: easyemailverification-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.easyemailverification.com/agents.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.easyemailverification.com/agents.md\nsources:\n- https://www.easyemailverification.com/agents.md\n- https://www.easyemailverification.com/en-US/guides/activecampaign\n- https://www.easyemailverification.com/en-US/guides/mautic\ndescription: Easy Email Verification authenticates API requests using an API key.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Send the key in the `X-API-Key` header (recommended). The `apikey` query parameter and the `Authorization` header also work; see the\n    API reference.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an account at https://dashboard.easyemailverification.com/register and generate an API key at https://dashboard.easyemailverification.com/apisettings.\nnote: OAuth authentication is mentioned for Mautic integration, but no token or authorization URLs are provided on the pages.\ndocs: https://www.easyemailverification.com/agents.md\n"
source_yaml_url: https://artifacts.apis.io/easyemailverification-com/authentication/easyemailverification-com-authentication.yml
summary_line: 1 scheme
tags:
- Email Verification
- Software-as-a-Service
- Data Validation
- Marketing
---
