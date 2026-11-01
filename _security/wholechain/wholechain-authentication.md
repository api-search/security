---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wholechain-connect-api-openapi.yml
  format: yaml
  label: Wholechain Connect API
  slug: wholechain-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-connect-api-openapi.yml
- filename: wholechain-edi-api-openapi.yml
  format: yaml
  label: Wholechain Edi API
  slug: wholechain-edi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-edi-api-openapi.yml
- filename: wholechain-epcis-interface-api-openapi.yml
  format: yaml
  label: Wholechain EPCIS Interface API
  slug: wholechain-epcis-interface-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-epcis-interface-api-openapi.yml
- filename: wholechain-epcis-legacy-interface-api-openapi.yml
  format: yaml
  label: Wholechain EPCIS Legacy Interface API
  slug: wholechain-epcis-legacy-interface-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-epcis-legacy-interface-api-openapi.yml
- filename: wholechain-events-api-openapi.yml
  format: yaml
  label: Wholechain Events API
  slug: wholechain-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-events-api-openapi.yml
- filename: wholechain-externaloauth-api-openapi.yml
  format: yaml
  label: Wholechain External O Auth API
  slug: wholechain-externaloauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-externaloauth-api-openapi.yml
- filename: wholechain-health-api-openapi.yml
  format: yaml
  label: Wholechain Health API
  slug: wholechain-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-health-api-openapi.yml
auth_types: []
description: Wholechain API uses API keys for authentication, which must be included in request headers.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Wholechain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wholechain declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Wholechain
provider_slug: wholechain
scheme_count: 1
schemes:
- evidence: The Wholechain API uses API keys as the primary method of authentication.
  header: Authorization
  how_to_obtain: 'Log into Your Wholechain Account: Use your credentials to log into your Wholechain platform account. Navigate to Settings: Once logged in, go to the settings section by clicking on the settings icon located in the top right corner of the dashboard. Account Settings: On the left-hand side panel, select Account Settings . Scroll Down to Integration Settings: In the Account Settings page, scroll to the bottom until you reach the section labeled Integration Settings . Generate Your API Key: Under Integration Settings , you will see an option labeled API Key . Click the Generate API Key button. This will generate a new API key for your account. Use Your API Key: Once the key is generated, you can copy it and use it in the headers of your API requests.'
  location: header
  name: API Key
  type: apiKey
slug: wholechain-authentication
source_filename: wholechain-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.wholechain.com/GettingStarted/Authentication/
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (deepseek)\nsource: https://developers.wholechain.com/GettingStarted/Authentication/\nsources:\n- https://developers.wholechain.com/GettingStarted/Authentication/\n- https://developers.wholechain.com/GettingStarted/Introduction/\n- https://developers.wholechain.com/GettingStarted/SandboxSetup/\ndescription: Wholechain API uses API keys for authentication, which must be included in request headers.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The Wholechain API uses API keys as the primary method of authentication.\n  header: Authorization\n  location: header\n  how_to_obtain: 'Log into Your Wholechain Account: Use your credentials to log into your Wholechain platform account. Navigate to Settings: Once\n    logged in, go to the settings section by clicking on the settings icon located in the top right corner of the dashboard. Account Settings:\n    On the left-hand side panel, select\
  \ Account Settings . Scroll Down to Integration Settings: In the Account Settings page, scroll to the bottom\n    until you reach the section labeled Integration Settings . Generate Your API Key: Under Integration Settings , you will see an option labeled\n    API Key . Click the Generate API Key button. This will generate a new API key for your account. Use Your API Key: Once the key is generated,\n    you can copy it and use it in the headers of your API requests.'\ndocs: https://developers.wholechain.com/GettingStarted/Authentication/\nnote: The documentation mentions using the API key \"in the headers of your API requests\" but doesn't specify the exact header name. The Authorization\n  header is a common convention for API keys, but the page doesn't explicitly state which header to use.\n"
source_yaml_url: https://artifacts.apis.io/wholechain/authentication/wholechain-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Supply Chain
- Traceability
- Blockchain
- Food Safety
- Compliance
- GS1
- Logistics
---
