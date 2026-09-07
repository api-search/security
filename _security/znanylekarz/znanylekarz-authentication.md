---
anonymous_access: false
api_key_in: []
api_specs:
- filename: znanylekarz-integrations-api.yml
  format: yaml
  label: Docplanner Integrations API
  slug: docplanner-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-integrations-api.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Znanylekarz Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ZnanyLekarz secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ZnanyLekarz
provider_slug: znanylekarz
scheme_count: 1
schemes:
- description: 'The API utilizes the industry-standard [OAuth 2.0](https://tools.ietf.org/html/rfc6749) protocol.


    All requests to our API must be authenticated and must include a valid access token.


    `NOTE! Our SSO Api version is v2 while our Integration Api version is v3`


    You can get a token for testing purposes with cURL


    ```

    curl -u {client_id}:{client_secret} https://www.{domain}/oauth/v2/token -d ''grant_ty'
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://www.{domain}/oauth/v2/token
  name: oauth2
  sources:
  - openapi/znanylekarz-integrations-api.yml
  type: oauth2
slug: znanylekarz-authentication
source_filename: znanylekarz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://integrations.docplanner.com/guide/fundamentals/authorization.html\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.{domain}/oauth/v2/token\n    scopes: 1\n  description: 'The API utilizes the industry-standard [OAuth 2.0](https://tools.ietf.org/html/rfc6749)\n    protocol.\n\n\n    All requests to our API must be authenticated and must include a valid access token.\n\n\n    `NOTE! Our SSO Api version is v2 while our Integration Api version is v3`\n\n\n    You can get a token for testing purposes with cURL\n\n\n    ```\n\n    curl -u {client_id}:{client_secret} https://www.{domain}/oauth/v2/token -d ''grant_ty'\n  sources:\n  - openapi/znanylekarz-integrations-api.yml\ndocs: https://integrations.docplanner.com/guide/fundamentals/authorization.html\nderived_from: openapi/znanylekarz-integrations-api.yml\n\
  note: 'Single-scheme API: OAuth 2.0 client_credentials only. No API-key header, no HTTP Basic on the resource\n  endpoints, no mutual TLS, no OpenID Connect. Credentials are issued per integration partner through\n  a manual onboarding, so there is no self-service key. Verified live on 2026-09-05: an unauthenticated\n  GET of https://www.znanylekarz.pl/api/v3/integration/facilities returns HTTP 401 with {\"message\":\"Authentication\n  credentials could not be found.\"}'\ntoken_endpoint_resolved: https://www.znanylekarz.pl/oauth/v2/token\ntoken_endpoint_templated: https://www.{domain}/oauth/v2/token\ntoken_lifetime_seconds: 3600\ntoken_type: bearer\nrefresh_token: false\nrequest_header: 'Authorization: Bearer {access_token}'\ntoken_exchange: HTTP Basic — curl -u {client_id}:{client_secret} ... -d grant_type=client_credentials&scope=integration\nsso_version_note: '\"NOTE! Our SSO Api version is v2 while our Integration Api version is v3\" — the token\n  endpoint lives under /oauth/v2/ while\
  \ the API lives under /api/v3/.'\nself_service: false\ncredential_issuance:\n  gated: true\n  audience: medical software providers\n  sandbox_first: true\n  contact: integrations@docplanner.com\n  source: https://integrations.docplanner.com/guide/integration-process.html\ndiscovery:\n  openid_configuration: false\n  oauth_authorization_server: false\n  note: No RFC 8414 authorization-server metadata and no OpenID Connect discovery document is served on\n    any host — both 404. The token endpoint is discoverable only by reading the OpenAPI securityScheme,\n    which means an agent cannot bootstrap auth from /.well-known/.\nlive_probe:\n  url: https://www.znanylekarz.pl/api/v3/integration/facilities\n  status: 401\n  body: '{\"message\":\"Authentication credentials could not be found.\"}'\n  checked: '2026-09-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/authentication/znanylekarz-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Healthcare
- Health Tech
- Appointments
- Booking
- Medical
- Marketplace
- Doctors
- Scheduling
- Poland
- Practice Management
- Telemedicine
---
