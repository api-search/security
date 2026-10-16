---
anonymous_access: false
api_key_in: []
api_specs:
- filename: unity-catalog-catalogs-api-openapi.yml
  format: yaml
  label: Unity Catalog Catalogs API
  slug: unity-catalog-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-catalogs-api-openapi.yml
- filename: unity-catalog-credentials-api-openapi.yml
  format: yaml
  label: Unity Catalog Credentials API
  slug: unity-catalog-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-credentials-api-openapi.yml
- filename: unity-catalog-deltacommits-api-openapi.yml
  format: yaml
  label: Unity Catalog Delta Commits API
  slug: unity-catalog-deltacommits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-deltacommits-api-openapi.yml
- filename: unity-catalog-external-locations-api-openapi.yml
  format: yaml
  label: Unity Catalog External Locations API
  slug: unity-catalog-external-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-external-locations-api-openapi.yml
- filename: unity-catalog-functions-api-openapi.yml
  format: yaml
  label: Unity Catalog Functions API
  slug: unity-catalog-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-functions-api-openapi.yml
- filename: unity-catalog-grants-api-openapi.yml
  format: yaml
  label: Unity Catalog Grants API
  slug: unity-catalog-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-grants-api-openapi.yml
- filename: unity-catalog-metastores-api-openapi.yml
  format: yaml
  label: Unity Catalog Metastores API
  slug: unity-catalog-metastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-metastores-api-openapi.yml
- filename: unity-catalog-schemas-api-openapi.yml
  format: yaml
  label: Unity Catalog Schemas API
  slug: unity-catalog-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-schemas-api-openapi.yml
- filename: unity-catalog-tables-api-openapi.yml
  format: yaml
  label: Unity Catalog Tables API
  slug: unity-catalog-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-tables-api-openapi.yml
- filename: unity-catalog-temporarycredentials-api-openapi.yml
  format: yaml
  label: Unity Catalog Temporary Credentials API
  slug: unity-catalog-temporarycredentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-temporarycredentials-api-openapi.yml
- filename: unity-catalog-volumes-api-openapi.yml
  format: yaml
  label: Unity Catalog Volumes API
  slug: unity-catalog-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-volumes-api-openapi.yml
- filename: unity-catalog-model-versions-api-openapi.yml
  format: yaml
  label: Unity Catalog Model Versions API
  slug: unity-catalog-model-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-model-versions-api-openapi.yml
- filename: unity-catalog-registered-models-api-openapi.yml
  format: yaml
  label: Unity Catalog Registered Models API
  slug: unity-catalog-registered-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/openapi/unity-catalog-registered-models-api-openapi.yml
auth_types: []
description: Authentication uses Google OAuth2 as configured in the Unity Catalog server.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Unity Catalog Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unity Catalog declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Unity Catalog
provider_slug: unity-catalog
scheme_count: 1
schemes:
- authorize_url: https://accounts.google.com/o/oauth2/auth
  evidence: server.authorization-url =https://accounts.google.com/o/oauth2/auth
  flows:
  - authorization_code
  how_to_obtain: Obtain a client ID and client secret from Google Cloud Console and set them in etc/conf/server.properties (server.client-id and server.client-secret).
  name: Google OAuth
  scopes:
  - openid
  - profile
  - email
  type: oauth2
slug: unity-catalog-authentication
source_filename: unity-catalog-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.unitycatalog.io/server/auth/
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.unitycatalog.io/server/auth/\nsources:\n- https://docs.unitycatalog.io/server/auth/\n- https://docs.unitycatalog.io/server/google-auth/\n- https://docs.unitycatalog.io/quickstart/\n- https://docs.unitycatalog.io/ai/quickstart/\ndescription: Authentication uses Google OAuth2 as configured in the Unity Catalog server.\nschemes:\n- type: oauth2\n  name: Google OAuth\n  evidence: server.authorization-url =https://accounts.google.com/o/oauth2/auth\n  flows:\n  - authorization_code\n  authorize_url: https://accounts.google.com/o/oauth2/auth\n  scopes:\n  - openid\n  - profile\n  - email\n  how_to_obtain: Obtain a client ID and client secret from Google Cloud Console and set them in etc/conf/server.properties (server.client-id and\n    server.client-secret).\ndocs: https://docs.unitycatalog.io/server/auth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unity-catalog/refs/heads/main/authentication/unity-catalog-authentication.yml
summary_line: 1 scheme
tags:
- Data
- AI
- Catalog
- Governance
- Multimodal
---
