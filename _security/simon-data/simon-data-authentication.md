---
api_key_in: []
api_specs:
- filename: simon-data-event-ingestion-openapi.yml
  format: yaml
  label: Simon Data Event Ingestion API
  slug: simon-data-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-event-ingestion-openapi.yml
- filename: simon-data-contact-openapi.yml
  format: yaml
  label: Simon Data Contact API
  slug: simon-data-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-contact-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Simon Data Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Simon Data secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Simon Data
provider_slug: simon-data
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication required for all endpoints.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.simondata.com/oauth/token
  name: oauth2
  sources:
  - openapi/simon-data-contact-openapi.yml
  type: oauth2
slug: simon-data-authentication
source_filename: simon-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simon-data-contact-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.simondata.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authentication required for all endpoints.\n  sources:\n  - openapi/simon-data-contact-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/authentication/simon-data-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Customer Data Platform
- CDP
- Marketing Automation
- Audience Segmentation
- Event Tracking
- Data Ingestion
- Personalization
- Marketing Technology
---
