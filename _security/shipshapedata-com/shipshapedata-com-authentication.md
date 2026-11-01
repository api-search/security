---
anonymous_access: true
api_key_in: []
api_specs:
- filename: shipshapedata-com-ai-readiness-api-openapi.yml
  format: yaml
  label: shipshapedata-com Ai Readiness API
  slug: shipshapedata-com-ai-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-ai-readiness-api-openapi.yml
- filename: shipshapedata-com-batch-api-openapi.yml
  format: yaml
  label: shipshapedata-com Batch API
  slug: shipshapedata-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-batch-api-openapi.yml
- filename: shipshapedata-com-case-studies-api-openapi.yml
  format: yaml
  label: shipshapedata-com Case Studies API
  slug: shipshapedata-com-case-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-case-studies-api-openapi.yml
- filename: shipshapedata-com-contact-api-openapi.yml
  format: yaml
  label: shipshapedata-com Contact API
  slug: shipshapedata-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-contact-api-openapi.yml
- filename: shipshapedata-com-export-api-openapi.yml
  format: yaml
  label: shipshapedata-com Export API
  slug: shipshapedata-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-export-api-openapi.yml
- filename: shipshapedata-com-industries-api-openapi.yml
  format: yaml
  label: shipshapedata-com Industries API
  slug: shipshapedata-com-industries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-industries-api-openapi.yml
- filename: shipshapedata-com-resources-api-openapi.yml
  format: yaml
  label: shipshapedata-com Resources API
  slug: shipshapedata-com-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-resources-api-openapi.yml
- filename: shipshapedata-com-services-api-openapi.yml
  format: yaml
  label: shipshapedata-com Services API
  slug: shipshapedata-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-services-api-openapi.yml
- filename: shipshapedata-com-shipshape-data-api-api-openapi.yml
  format: yaml
  label: shipshapedata-com Shipshape Data API
  slug: shipshapedata-com-shipshape-data-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-shipshape-data-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Shipshapedata Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: shipshapedata-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: shipshapedata-com
provider_slug: shipshapedata-com
scheme_count: 2
schemes:
- description: Public read endpoints are unauthenticated.
  type: none
- description: OAuth 2.0 client credentials grant for bulk export.
  flows:
    clientCredentials:
      scopes:
        export: Access to bulk export endpoint.
      tokenUrl: https://shipshapedata.com/oauth/token
  type: oauth2
slug: shipshapedata-com-authentication
source_filename: shipshapedata-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://shipshapedata.com/auth.md\nschemes:\n  - type: none\n    description: Public read endpoints are unauthenticated.\n  - type: oauth2\n    description: OAuth 2.0 client credentials grant for bulk export.\n    flows:\n      clientCredentials:\n        tokenUrl: https://shipshapedata.com/oauth/token\n        scopes:\n          export: Access to bulk export endpoint.\n"
source_yaml_url: https://artifacts.apis.io/shipshapedata-com/authentication/shipshapedata-com-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Data
- Consultancy
- London
- API
---
