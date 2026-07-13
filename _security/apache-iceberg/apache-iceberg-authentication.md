---
api_key_in: []
api_specs:
- filename: apache-iceberg-rest-catalog-open-api.yaml
  format: yaml
  label: Apache Iceberg REST Catalog API
  slug: rest-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/openapi/apache-iceberg-rest-catalog-open-api.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Apache Iceberg Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Apache Iceberg secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Apache Iceberg
provider_slug: apache-iceberg
scheme_count: 2
schemes:
- description: 'This scheme is used for OAuth2 authorization.


    For unauthorized requests, services should return an appropriate 401 or 403 response. Implementations must not return altered success (200) responses when a request is unauthenticated or unauthorized.

    If a separate authorization server is used, substitute the tokenUrl with the full token path of the external authorization server, and use the resulting'
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /v1/oauth/tokens
  name: OAuth2
  sources:
  - openapi/apache-iceberg-rest-catalog-open-api.yaml
  type: oauth2
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/apache-iceberg-rest-catalog-open-api.yaml
  type: http
slug: apache-iceberg-authentication
source_filename: apache-iceberg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-iceberg-rest-catalog-open-api.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth/tokens\n    scopes: 1\n  description: |-\n    This scheme is used for OAuth2 authorization.\n\n    For unauthorized requests, services should return an appropriate 401 or 403 response. Implementations must not return altered success (200) responses when a request is unauthenticated or unauthorized.\n    If a separate authorization server is used, substitute the tokenUrl with the full token path of the external authorization server, and use the resulting\n  sources:\n  - openapi/apache-iceberg-rest-catalog-open-api.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/apache-iceberg-rest-catalog-open-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/authentication/apache-iceberg-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
---
