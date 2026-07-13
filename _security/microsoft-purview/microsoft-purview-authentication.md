---
api_key_in: []
api_specs:
- filename: microsoft-purview-catalog-openapi.yml
  format: yaml
  label: Microsoft Purview Catalog API
  slug: microsoft-purview-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-catalog-openapi.yml
- filename: microsoft-purview-scanning-openapi.yml
  format: yaml
  label: Microsoft Purview Scanning API
  slug: microsoft-purview-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-scanning-openapi.yml
- filename: microsoft-purview-account-openapi.yml
  format: yaml
  label: Microsoft Purview Account API
  slug: microsoft-purview-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-account-openapi.yml
- filename: microsoft-purview-data-map-openapi.yml
  format: yaml
  label: Microsoft Purview Data Map API
  slug: microsoft-purview-data-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-data-map-openapi.yml
- filename: microsoft-purview-metadata-policies-openapi.yml
  format: yaml
  label: Microsoft Purview Metadata Policies API
  slug: microsoft-purview-metadata-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-metadata-policies-openapi.yml
- filename: microsoft-purview-workflow-openapi.yml
  format: yaml
  label: Microsoft Purview Workflow API
  slug: microsoft-purview-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-workflow-openapi.yml
- filename: microsoft-purview-unified-catalog-openapi.yml
  format: yaml
  label: Microsoft Purview Unified Catalog API
  slug: microsoft-purview-unified-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-unified-catalog-openapi.yml
- filename: microsoft-purview-data-quality-openapi.yml
  format: yaml
  label: Microsoft Purview Data Quality API
  slug: microsoft-purview-data-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-data-quality-openapi.yml
- filename: microsoft-purview-ediscovery-openapi.yml
  format: yaml
  label: Microsoft Purview eDiscovery API
  slug: microsoft-purview-ediscovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-ediscovery-openapi.yml
- filename: microsoft-purview-information-protection-openapi.yml
  format: yaml
  label: Microsoft Purview Information Protection API
  slug: microsoft-purview-information-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-information-protection-openapi.yml
- filename: microsoft-purview-data-security-governance-openapi.yml
  format: yaml
  label: Microsoft Purview Data Security and Governance API
  slug: microsoft-purview-data-security-and-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-data-security-governance-openapi.yml
- filename: microsoft-purview-records-management-openapi.yml
  format: yaml
  label: Microsoft Purview Records Management API
  slug: microsoft-purview-records-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/openapi/microsoft-purview-records-management-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Purview Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft Purview secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft Purview
provider_slug: microsoft-purview
scheme_count: 2
schemes:
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-purview-account-openapi.yml
  - openapi/microsoft-purview-catalog-openapi.yml
  - openapi/microsoft-purview-data-map-openapi.yml
  - openapi/microsoft-purview-data-quality-openapi.yml
  - openapi/microsoft-purview-data-security-governance-openapi.yml
  - openapi/microsoft-purview-metadata-policies-openapi.yml
  - openapi/microsoft-purview-records-management-openapi.yml
  - openapi/microsoft-purview-scanning-openapi.yml
  - openapi/microsoft-purview-unified-catalog-openapi.yml
  - openapi/microsoft-purview-workflow-openapi.yml
  type: oauth2
- description: Microsoft Identity Platform OAuth2
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-purview-ediscovery-openapi.yml
  - openapi/microsoft-purview-information-protection-openapi.yml
  type: oauth2
slug: microsoft-purview-authentication
source_filename: microsoft-purview-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-purview-account-openapi.yml, openapi/microsoft-purview-catalog-openapi.yml,\n  openapi/microsoft-purview-data-map-openapi.yml, openapi/microsoft-purview-data-quality-openapi.yml,\n  openapi/microsoft-purview-data-security-governance-openapi.yml, openapi/microsoft-purview-ediscovery-openapi.yml,\n  openapi/microsoft-purview-information-protection-openapi.yml, openapi/microsoft-purview-metadata-policies-openapi.yml,\n  openapi/microsoft-purview-records-management-openapi.yml, openapi/microsoft-purview-scanning-openapi.yml,\n  openapi/microsoft-purview-unified-catalog-openapi.yml, openapi/microsoft-purview-workflow-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: Azure\
  \ Active Directory OAuth2 authentication\n  sources:\n  - openapi/microsoft-purview-account-openapi.yml\n  - openapi/microsoft-purview-catalog-openapi.yml\n  - openapi/microsoft-purview-data-map-openapi.yml\n  - openapi/microsoft-purview-data-quality-openapi.yml\n  - openapi/microsoft-purview-data-security-governance-openapi.yml\n  - openapi/microsoft-purview-metadata-policies-openapi.yml\n  - openapi/microsoft-purview-records-management-openapi.yml\n  - openapi/microsoft-purview-scanning-openapi.yml\n  - openapi/microsoft-purview-unified-catalog-openapi.yml\n  - openapi/microsoft-purview-workflow-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 2\n  description: Microsoft Identity Platform OAuth2\n  sources:\n  - openapi/microsoft-purview-ediscovery-openapi.yml\n  - openapi/microsoft-purview-information-protection-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/authentication/microsoft-purview-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
---
