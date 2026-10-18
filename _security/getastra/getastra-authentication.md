---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getastra-openapi-generated.yml
  format: yaml
  label: Astra Pentest API
  slug: getastra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getastra/refs/heads/main/openapi/_ae-authored/getastra-openapi-generated.yml
auth_types: []
description: Authentication schemes supported by Astra for API targets
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Getastra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Astra Pentest declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Astra Pentest
provider_slug: getastra
scheme_count: 2
schemes:
- evidence: Select JWT Bearer as the authentication type.
  header: Authorization
  how_to_obtain: Astra generates the JWT token using the configured signing algorithm, secret/key, payload and header.
  location: header
  name: JWT Bearer
  type: http-bearer
- evidence: From the Authentication Type dropdown, select OAuth 2.0.
  how_to_obtain: Provide Access Token URL, Client ID, Client Secret (and optionally Username/Password for Resource Owner Password grant). Astra uses these to obtain tokens automatically.
  name: OAuth 2.0
  token_url: https://example.com/login/oauth/access_token
  type: oauth2
slug: getastra-authentication
source_filename: getastra-authentication.yml
source_heading: Authentication Profile
source_url: https://help.getastra.com/articles/8634520513-how-to-provide-jwt-configuration-for-automated-authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.getastra.com/articles/8634520513-how-to-provide-jwt-configuration-for-automated-authentication\nsources:\n- https://help.getastra.com/articles/8634520513-how-to-provide-jwt-configuration-for-automated-authentication\n- https://help.getastra.com/articles/2951300258-how-to-provide-oauth-2-0-authentication-details-for-secure-api-access\n- https://help.getastra.com/articles/4242572340-how-to-verify-credentials-in-your-postman-collection\n- https://help.getastra.com/articles/2492056622-what-are-the-steps-involved-in-signing-a-android-application\ndescription: Authentication schemes supported by Astra for API targets\nschemes:\n- type: http-bearer\n  name: JWT Bearer\n  evidence: Select JWT Bearer as the authentication type.\n  location: header\n  header: Authorization\n  how_to_obtain: Astra generates the JWT token using the configured signing algorithm, secret/key, payload\
  \ and header.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: From the Authentication Type dropdown, select OAuth 2.0.\n  token_url: https://example.com/login/oauth/access_token\n  how_to_obtain: Provide Access Token URL, Client ID, Client Secret (and optionally Username/Password for Resource Owner Password grant). Astra\n    uses these to obtain tokens automatically.\ndocs: https://help.getastra.com/articles/8634520513-how-to-provide-jwt-configuration-for-automated-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getastra/refs/heads/main/authentication/getastra-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- PenetrationTesting
- API
- Cloud
---
