---
api_key_in: []
api_specs:
- filename: process
  format: yaml
  label: Sentinel Hub Process API
  slug: process
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/process
- filename: catalog
  format: yaml
  label: Sentinel Hub Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/catalog
- filename: statistical
  format: yaml
  label: Sentinel Hub Statistical API
  slug: statistical
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/statistical
- filename: batch_process
  format: yaml
  label: Sentinel Hub Batch Processing API
  slug: batch
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/batch_process
- filename: byoc
  format: yaml
  label: Sentinel Hub BYOC API
  slug: byoc
  spec_type: OpenAPI
  url: https://docs.sentinel-hub.com/api/latest/reference/#tag/byoc
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sentinel Hub Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sentinel Hub secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sentinel Hub
provider_slug: sentinel-hub
scheme_count: 1
schemes:
- description: "### Authentication\n\nMore about the authentication <a href=\"https://docs.planet.com/develop/authentication/\" target=\"_blank\">here</a>.\n\nTo get an access token using curl:\n\n```\ncurl --request POST \\\n  --url https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token \\\n  --header \"content-type: application/x-www-form-urlencoded\" \\\n  --data \"grant_type=client_credentials&client_id"
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token
  name: OAuth2
  sources:
  - openapi/sentinel-hub-openapi.yaml
  type: oauth2
slug: sentinel-hub-authentication
source_filename: sentinel-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sentinel-hub-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token\n    scopes: 1\n  description: |-\n    ### Authentication\n\n    More about the authentication <a href=\"https://docs.planet.com/develop/authentication/\" target=\"_blank\">here</a>.\n\n    To get an access token using curl:\n\n    ```\n    curl --request POST \\\n      --url https://services.sentinel-hub.com/auth/realms/main/protocol/openid-connect/token \\\n      --header \"content-type: application/x-www-form-urlencoded\" \\\n      --data \"grant_type=client_credentials&client_id\n  sources:\n  - openapi/sentinel-hub-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentinel-hub/refs/heads/main/authentication/sentinel-hub-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Satellite Imagery
- Geospatial
- Remote Sensing
- Earth Observation
- NDVI
- Sentinel
- Landsat
- MODIS
- OGC
- STAC
---
