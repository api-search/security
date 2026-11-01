---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Symmetry products as documented.
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Symmetry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Symmetry declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Symmetry
provider_slug: symmetry
scheme_count: 5
schemes:
- evidence: To use basic authentication in the schema for proxy endpoints, set the "authType" value to "BASIC" within the nested webservice.proxy.authentication element
  header: Authorization
  how_to_obtain: Provide username and password in the proxy authentication configuration.
  location: header
  name: Basic authentication for proxy endpoints
  type: http-basic
- evidence: To use OAuth 2.0 authentication using grant type client credentials in the schema for postback data, configure your SPF Registration
  how_to_obtain: Set oauth2GrantType to CLIENT_CREDENTIALS and provide oauth2ClientId, oauth2ClientSecret, and oauth2AuthServerUrl in the registration.
  name: OAuth 2.0 client credentials for postback data
  type: oauth2
- evidence: To use OAuth 2.0 authentication using grant type password credentials in the schema for postback data, configure your SPF Registration
  how_to_obtain: Set oauth2GrantType to PASSWORD and provide oauth2ClientId, oauth2ClientSecret, username, password, and oauth2AuthServerUrl in the registration.
  name: OAuth 2.0 password grant for postback data
  type: oauth2
- authorize_url: https://api.symmetry.com/authentication/login
  evidence: The encrypted JWT token is to be included in each request to the SPF-API as a Bearer token in the Authorization header
  header: Authorization
  how_to_obtain: Make a GET request to https://api.symmetry.com/authentication/login with the api-key header containing your API Key or Hash; the response returns an accessToken.
  location: header
  name: JWT bearer token for SPF API
  type: http-bearer
- authorize_url: https://api.symmetry.com/authentication/login
  evidence: To request a new JWT access token, make an HTTP GET request to the URL below, setting the api-key header to the API Key or Hash provided by Symmetry.
  header: api-key
  how_to_obtain: Include the provided API key in the api-key header when calling the login endpoint; the response returns an accessToken used as a Bearer token.
  location: header
  name: API key for I‑9 login endpoint
  type: apiKey
slug: symmetry-authentication
source_filename: symmetry-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.symmetry.com/spf/getting-started/authentication.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.symmetry.com/spf/getting-started/authentication.md\nsources:\n- https://docs.symmetry.com/spf/getting-started/authentication.md\n- https://docs.symmetry.com/i9/core-concepts/authentication.md\n- https://docs.symmetry.com/cbs/core-concepts/authentication-model.md\n- https://docs.symmetry.com/i9/api-reference/admin/generate-a-token-for-an-admin-to-access-the-i9-system.md\ndescription: Authentication schemes for Symmetry products as documented.\nschemes:\n- type: http-basic\n  name: Basic authentication for proxy endpoints\n  evidence: To use basic authentication in the schema for proxy endpoints, set the \"authType\" value to \"BASIC\" within the nested webservice.proxy.authentication\n    element\n  location: header\n  header: Authorization\n  how_to_obtain: Provide username and password in the proxy authentication configuration.\n- type: oauth2\n  name: OAuth 2.0 client\
  \ credentials for postback data\n  evidence: To use OAuth 2.0 authentication using grant type client credentials in the schema for postback data, configure your SPF Registration\n  how_to_obtain: Set oauth2GrantType to CLIENT_CREDENTIALS and provide oauth2ClientId, oauth2ClientSecret, and oauth2AuthServerUrl in the registration.\n- type: oauth2\n  name: OAuth 2.0 password grant for postback data\n  evidence: To use OAuth 2.0 authentication using grant type password credentials in the schema for postback data, configure your SPF Registration\n  how_to_obtain: Set oauth2GrantType to PASSWORD and provide oauth2ClientId, oauth2ClientSecret, username, password, and oauth2AuthServerUrl in\n    the registration.\n- type: http-bearer\n  name: JWT bearer token for SPF API\n  evidence: The encrypted JWT token is to be included in each request to the SPF-API as a Bearer token in the Authorization header\n  location: header\n  header: Authorization\n  authorize_url: https://api.symmetry.com/authentication/login\n\
  \  how_to_obtain: Make a GET request to https://api.symmetry.com/authentication/login with the api-key header containing your API Key or Hash;\n    the response returns an accessToken.\n- type: apiKey\n  name: API key for I‑9 login endpoint\n  evidence: To request a new JWT access token, make an HTTP GET request to the URL below, setting the api-key header to the API Key or Hash provided\n    by Symmetry.\n  location: header\n  header: api-key\n  authorize_url: https://api.symmetry.com/authentication/login\n  how_to_obtain: Include the provided API key in the api-key header when calling the login endpoint; the response returns an accessToken used\n    as a Bearer token.\ndocs: https://docs.symmetry.com/spf/getting-started/authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/symmetry/authentication/symmetry-authentication.yml
summary_line: 5 schemes
tags:
- Payroll Tax Compliance
- Payroll Platforms
- EOR
- PEO
- Recruiting
- Staffing
- Large Employers
- Tax APIs
---
