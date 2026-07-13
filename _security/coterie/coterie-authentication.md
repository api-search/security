---
api_key_in: []
api_specs:
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Quotes API
  slug: coterie-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Policies API
  slug: coterie-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Applications API
  slug: coterie-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Industry / NAICS API
  slug: coterie-industry-naics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Documents API
  slug: coterie-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Webhooks API
  slug: coterie-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Coterie Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Coterie Insurance secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Coterie Insurance
provider_slug: coterie
scheme_count: 2
schemes:
- description: Pass your Coterie API key as a Bearer token in the Authorization header. Channel partners are issued a Publishable Key (client-side) and a Secret Key (server-side only); some operations require the Secret Key. Partners may also authenticate via OAuth2 client-credentials to obtain a Bearer access token. Producer attribution uses the token producer_{producerId} form.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/coterie-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token
  name: oauth2
  sources:
  - openapi/coterie-openapi.yml
  type: oauth2
slug: coterie-authentication
source_filename: coterie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coterie-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Pass your Coterie API key as a Bearer token in the Authorization header. Channel\n    partners are issued a Publishable Key (client-side) and a Secret Key (server-side only);\n    some operations require the Secret Key. Partners may also authenticate via OAuth2 client-credentials\n    to obtain a Bearer access token. Producer attribution uses the token producer_{producerId}\n    form.\n  sources:\n  - openapi/coterie-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.coterieinsurance.com/v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/coterie-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/authentication/coterie-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Insurance
- Commercial Insurance
- Small Business
- Embedded Insurance
- Insurtech
---
