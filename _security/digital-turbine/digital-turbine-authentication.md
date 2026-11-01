---
anonymous_access: false
api_key_in: []
api_specs:
- filename: digital-turbine-openapi-generated.yml
  format: yaml
  label: Digital Turbine (Fyber) API
  slug: digital-turbine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digital-turbine/openapi/_ae-authored/digital-turbine-openapi-generated.yml
auth_types: []
description: Authentication schemes for Digital Turbine (Fyber) APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Digital Turbine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digital Turbine (Fyber) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Digital Turbine (Fyber)
provider_slug: digital-turbine
scheme_count: 2
schemes:
- evidence: Use the UI Management API credentials to authenticate your user and get back an access token to authorize further requests.
  flows:
  - client_credentials
  how_to_obtain: Copy both the Client ID and Client Secret keys from the Management API - Credentials section in the DT Console and include them in the POST request body as shown in the documentation.
  name: DT Management API OAuth2
  token_url: https://console.fyber.com/api/v2/management/auth
  type: oauth2
- evidence: Use the `auth/v1/token` endpoint to request an authorization token for the Offerwall Reporting API.
  flows:
  - client_credentials
  how_to_obtain: Send a POST request with JSON body containing `grant_type`, `client_id`, and `client_secret` to the token endpoint as shown in the sample request.
  name: Offerwall Reporting API OAuth2
  token_url: https://reporting.fyber.com/auth/v1/token
  type: oauth2
slug: digital-turbine-authentication
source_filename: digital-turbine-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.digitalturbine.com/dt-exchange/getting-started-with-dt-exchange/advanced-configurations/dt-exchange-management-api/authentication.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.digitalturbine.com/dt-exchange/getting-started-with-dt-exchange/advanced-configurations/dt-exchange-management-api/authentication.md\nsources:\n- https://docs.digitalturbine.com/dt-exchange/getting-started-with-dt-exchange/advanced-configurations/dt-exchange-management-api/authentication.md\n- https://docs.digitalturbine.com/dt-fairbid/reporting/reporting-api/api-authentication.md\n- https://docs.digitalturbine.com/dt-fairbid/advanced-configurations/dt-fairbid-management-api/authentication.md\n- https://docs.digitalturbine.com/dt-offer-wall/reporting/reporting-api/auth-v1-token.md\ndescription: Authentication schemes for Digital Turbine (Fyber) APIs\nschemes:\n- type: oauth2\n  name: DT Management API OAuth2\n  evidence: Use the UI Management API credentials to authenticate your user and get back an access token to authorize further requests.\n  flows:\n  - client_credentials\n\
  \  token_url: https://console.fyber.com/api/v2/management/auth\n  how_to_obtain: Copy both the Client ID and Client Secret keys from the Management API - Credentials section in the DT Console and include them\n    in the POST request body as shown in the documentation.\n- type: oauth2\n  name: Offerwall Reporting API OAuth2\n  evidence: Use the `auth/v1/token` endpoint to request an authorization token for the Offerwall Reporting API.\n  flows:\n  - client_credentials\n  token_url: https://reporting.fyber.com/auth/v1/token\n  how_to_obtain: Send a POST request with JSON body containing `grant_type`, `client_id`, and `client_secret` to the token endpoint as shown in\n    the sample request.\ndocs: https://docs.digitalturbine.com/dt-exchange/getting-started-with-dt-exchange/advanced-configurations/dt-exchange-management-api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/digital-turbine/authentication/digital-turbine-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Mobile
- Advertising
- Monetization
- SDK
---
