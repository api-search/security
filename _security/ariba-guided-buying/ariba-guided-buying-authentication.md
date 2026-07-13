---
api_key_in: []
api_specs:
- filename: ariba-guided-buying-catalog-shop-api.yaml
  format: yaml
  label: Ariba Guided Buying - Public Catalogs Shop API
  slug: ariba-guided-buying-catalog-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/openapi/ariba-guided-buying-catalog-shop-api.yaml
- filename: ariba-guided-buying-asset-management-api.yaml
  format: yaml
  label: Ariba Guided Buying - Asset Management API
  slug: ariba-guided-buying-asset-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/openapi/ariba-guided-buying-asset-management-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ariba Guided Buying Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ariba Guided Buying secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token using client credentials.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: OAuth2
  sources:
  - openapi/ariba-guided-buying-asset-management-api.yaml
  - openapi/ariba-guided-buying-catalog-shop-api.yaml
  type: oauth2
slug: ariba-guided-buying-authentication
source_filename: ariba-guided-buying-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ariba-guided-buying-asset-management-api.yaml, openapi/ariba-guided-buying-catalog-shop-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials.\n  sources:\n  - openapi/ariba-guided-buying-asset-management-api.yaml\n  - openapi/ariba-guided-buying-catalog-shop-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/authentication/ariba-guided-buying-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
---
