---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hedgespecialty-com-account-api-openapi.yml
  format: yaml
  label: Hedge Account API
  slug: hedgespecialty-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-account-api-openapi.yml
- filename: hedgespecialty-com-appetite-api-openapi.yml
  format: yaml
  label: Hedge Appetite API
  slug: hedgespecialty-com-appetite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-appetite-api-openapi.yml
- filename: hedgespecialty-com-auth-api-openapi.yml
  format: yaml
  label: Hedge Auth API
  slug: hedgespecialty-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-auth-api-openapi.yml
- filename: hedgespecialty-com-binding-api-openapi.yml
  format: yaml
  label: Hedge Binding API
  slug: hedgespecialty-com-binding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-binding-api-openapi.yml
- filename: hedgespecialty-com-carrier-quotes-api-openapi.yml
  format: yaml
  label: Hedge Carrier quotes API
  slug: hedgespecialty-com-carrier-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-carrier-quotes-api-openapi.yml
- filename: hedgespecialty-com-documents-api-openapi.yml
  format: yaml
  label: Hedge Documents API
  slug: hedgespecialty-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-documents-api-openapi.yml
- filename: hedgespecialty-com-market-access-api-openapi.yml
  format: yaml
  label: Hedge Market access API
  slug: hedgespecialty-com-market-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-market-access-api-openapi.yml
- filename: hedgespecialty-com-payments-api-openapi.yml
  format: yaml
  label: Hedge Payments API
  slug: hedgespecialty-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-payments-api-openapi.yml
- filename: hedgespecialty-com-policies-api-openapi.yml
  format: yaml
  label: Hedge Policies API
  slug: hedgespecialty-com-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-policies-api-openapi.yml
- filename: hedgespecialty-com-programs-api-openapi.yml
  format: yaml
  label: Hedge Programs API
  slug: hedgespecialty-com-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-programs-api-openapi.yml
- filename: hedgespecialty-com-requirements-api-openapi.yml
  format: yaml
  label: Hedge Requirements API
  slug: hedgespecialty-com-requirements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-requirements-api-openapi.yml
- filename: hedgespecialty-com-submissions-api-openapi.yml
  format: yaml
  label: Hedge Submissions API
  slug: hedgespecialty-com-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-submissions-api-openapi.yml
- filename: hedgespecialty-com-webhooks-api-openapi.yml
  format: yaml
  label: Hedge Webhooks API
  slug: hedgespecialty-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-webhooks-api-openapi.yml
auth_types: []
description: Hedge uses OAuth 2.0 for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hedgespecialty Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hedge declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hedge
provider_slug: hedgespecialty-com
scheme_count: 1
schemes:
- authorize_url: https://api.hedgespecialty.com/api/v1/oauth/authorize
  evidence: RFC 6749 authorization endpoint, PKCE (S256) required. Redirects the broker to the portal consent screen; on approval the browser returns to your redirect_uri with a single-use code for /oauth/token.
  flows:
  - authorization_code
  - client_credentials
  - device_code
  how_to_obtain: Register a client via POST /oauth/register to receive a client_id (no client_secret). Use the client_id with the authorization endpoint or device authorization endpoint, then exchange the code or device code at POST /oauth/token.
  name: OAuth2
  type: oauth2
slug: hedgespecialty-com-authentication
source_filename: hedgespecialty-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hedgespecialty.com/api/operations/registeroauthclient
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hedgespecialty.com/api/operations/registeroauthclient\nsources:\n- https://docs.hedgespecialty.com/api/operations/registeroauthclient\n- https://docs.hedgespecialty.com/api/operations/startoauthauthorization\n- https://docs.hedgespecialty.com/api/operations/startoauthdeviceauthorization\n- https://docs.hedgespecialty.com/api/operations/exchangeoauthtoken\ndescription: Hedge uses OAuth 2.0 for authentication.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: RFC 6749 authorization endpoint, PKCE (S256) required. Redirects the broker to the portal consent screen; on approval the browser\n    returns to your redirect_uri with a single-use code for /oauth/token.\n  flows:\n  - authorization_code\n  - client_credentials\n  - device_code\n  authorize_url: https://api.hedgespecialty.com/api/v1/oauth/authorize\n  how_to_obtain: Register a client via POST /oauth/register\
  \ to receive a client_id (no client_secret). Use the client_id with the authorization\n    endpoint or device authorization endpoint, then exchange the code or device code at POST /oauth/token.\nnote: The documentation does not specify a header name for sending the access token; typical usage is the Authorization header with a Bearer token.\ndocs: https://docs.hedgespecialty.com/api/operations/registeroauthclient\n"
source_yaml_url: https://artifacts.apis.io/hedgespecialty-com/authentication/hedgespecialty-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Insurance
- Wholesale
- Brokers
- Specialty
---
