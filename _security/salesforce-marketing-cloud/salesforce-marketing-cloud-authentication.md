---
api_key_in: []
api_specs:
- filename: salesforce-marketing-cloud-openapi.yml
  format: yaml
  label: Marketing Cloud REST API
  slug: marketing-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/openapi/salesforce-marketing-cloud-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Marketing Cloud Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Salesforce Marketing Cloud secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
scheme_count: 1
schemes:
- description: Marketing Cloud uses OAuth 2.0 client credentials flow for authentication. Obtain a client ID and secret from an installed package in Marketing Cloud Setup, then exchange them for an access token at the authentication endpoint.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://YOUR_SUBDOMAIN.auth.marketingcloudapis.com/v2/token
  name: OAuth2
  sources:
  - openapi/salesforce-marketing-cloud-openapi.yml
  type: oauth2
slug: salesforce-marketing-cloud-authentication
source_filename: salesforce-marketing-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-marketing-cloud-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://YOUR_SUBDOMAIN.auth.marketingcloudapis.com/v2/token\n    scopes: 0\n  description: Marketing Cloud uses OAuth 2.0 client credentials flow for authentication. Obtain\n    a client ID and secret from an installed package in Marketing Cloud Setup, then exchange\n    them for an access token at the authentication endpoint.\n  sources:\n  - openapi/salesforce-marketing-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/authentication/salesforce-marketing-cloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
---
