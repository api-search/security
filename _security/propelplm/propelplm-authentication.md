---
api_key_in: []
api_specs:
- filename: propelplm-assembly-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Assembly API
  slug: propelplm-assembly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-assembly-api-openapi.yml
- filename: propelplm-assets-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) assets API
  slug: propelplm-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-assets-api-openapi.yml
- filename: propelplm-attachment-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Attachment API
  slug: propelplm-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-attachment-api-openapi.yml
- filename: propelplm-bill-of-material-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Bill of Material API
  slug: propelplm-bill-of-material-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-bill-of-material-api-openapi.yml
- filename: propelplm-bom-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) BOM API
  slug: propelplm-bom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-bom-api-openapi.yml
- filename: propelplm-categories-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) categories API
  slug: propelplm-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-categories-api-openapi.yml
- filename: propelplm-change-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) change API
  slug: propelplm-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-change-api-openapi.yml
- filename: propelplm-channels-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) channels API
  slug: propelplm-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-channels-api-openapi.yml
- filename: propelplm-configuration-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Configuration API
  slug: propelplm-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-configuration-api-openapi.yml
- filename: propelplm-item-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Item API
  slug: propelplm-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-item-api-openapi.yml
- filename: propelplm-manufactureritem-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) ManufacturerItem API
  slug: propelplm-manufactureritem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-manufactureritem-api-openapi.yml
- filename: propelplm-manufacturerpart-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) ManufacturerPart API
  slug: propelplm-manufacturerpart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-manufacturerpart-api-openapi.yml
- filename: propelplm-markup-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) markup API
  slug: propelplm-markup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-markup-api-openapi.yml
- filename: propelplm-products-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) products API
  slug: propelplm-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-products-api-openapi.yml
- filename: propelplm-variants-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) variants API
  slug: propelplm-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-variants-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Propelplm Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Propel Software (Propel PLM) secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Propel Software (Propel PLM)
provider_slug: propelplm
scheme_count: 2
schemes:
- description: This API uses OAuth 2 with the implicit grant flow.
  flows:
  - authorizationUrl: '{{url}}{{site}}/services/oauth2/authorize'
    flow: implicit
    scopes: 1
  name: oAuth2Implicit
  sources:
  - openapi/propelplm-configuration-openapi.yml
  - openapi/propelplm-manufacturer-item-openapi.yml
  - openapi/propelplm-manufacturer-part-openapi.yml
  type: oauth2
- description: Salesforce OAuth 2.0 (Connected App). Server-side (authorization code) flow.
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: salesforceOAuth
  sources:
  - openapi/propelplm-core-openapi.yml
  - openapi/propelplm-pim-openapi.yml
  type: oauth2
slug: propelplm-authentication
source_filename: propelplm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/propelplm-configuration-openapi.yml, openapi/propelplm-core-openapi.yml, openapi/propelplm-manufacturer-item-openapi.yml,\n  openapi/propelplm-manufacturer-part-openapi.yml, openapi/propelplm-pim-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: oAuth2Implicit\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: '{{url}}{{site}}/services/oauth2/authorize'\n    scopes: 1\n  description: This API uses OAuth 2 with the implicit grant flow.\n  sources:\n  - openapi/propelplm-configuration-openapi.yml\n  - openapi/propelplm-manufacturer-item-openapi.yml\n  - openapi/propelplm-manufacturer-part-openapi.yml\n- name: salesforceOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 4\n\
  \  description: Salesforce OAuth 2.0 (Connected App). Server-side (authorization code) flow.\n  sources:\n  - openapi/propelplm-core-openapi.yml\n  - openapi/propelplm-pim-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/authentication/propelplm-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Product Lifecycle Management
- PLM
- Quality Management
- QMS
- Product Information Management
- PIM
- Manufacturing
- Salesforce
- Bill of Materials
- Change Management
---
