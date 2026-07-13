---
api_key_in: []
api_specs:
- filename: salesforce-experience-cloud-sites-openapi.yml
  format: yaml
  label: Experience Cloud Sites API
  slug: experience-cloud-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-sites-openapi.yml
- filename: salesforce-experience-cloud-connect-communities-openapi.yml
  format: yaml
  label: Connect REST API (Communities)
  slug: connect-rest-api-communities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-connect-communities-openapi.yml
- filename: salesforce-experience-cloud-cms-connect-openapi.yml
  format: yaml
  label: CMS Connect API
  slug: cms-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-cms-connect-openapi.yml
- filename: salesforce-experience-cloud-rest-api-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-rest-api-openapi.yml
- filename: salesforce-experience-cloud-templates-openapi.yml
  format: yaml
  label: Experience Cloud Templates API
  slug: experience-cloud-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-templates-openapi.yml
- filename: salesforce-experience-cloud-graphql-openapi.yml
  format: yaml
  label: GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-graphql-openapi.yml
- filename: salesforce-experience-cloud-cms-managed-content-openapi.yml
  format: yaml
  label: CMS Managed Content API
  slug: cms-managed-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml
- filename: salesforce-experience-cloud-cms-delivery-openapi.yml
  format: yaml
  label: CMS Delivery API
  slug: cms-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-cms-delivery-openapi.yml
- filename: salesforce-experience-cloud-user-interface-openapi.yml
  format: yaml
  label: User Interface API
  slug: user-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-user-interface-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Experience Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Experience Cloud secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
scheme_count: 2
schemes:
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-experience-cloud-cms-connect-openapi.yml
  - openapi/salesforce-experience-cloud-cms-delivery-openapi.yml
  - openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml
  - openapi/salesforce-experience-cloud-connect-communities-openapi.yml
  - openapi/salesforce-experience-cloud-graphql-openapi.yml
  - openapi/salesforce-experience-cloud-rest-api-openapi.yml
  - openapi/salesforce-experience-cloud-sites-openapi.yml
  - openapi/salesforce-experience-cloud-templates-openapi.yml
  - openapi/salesforce-experience-cloud-user-interface-openapi.yml
  type: oauth2
- bearerFormat: OAuth2
  description: Bearer token obtained through OAuth 2.0 flow
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-experience-cloud-cms-connect-openapi.yml
  - openapi/salesforce-experience-cloud-cms-delivery-openapi.yml
  - openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml
  - openapi/salesforce-experience-cloud-connect-communities-openapi.yml
  - openapi/salesforce-experience-cloud-graphql-openapi.yml
  - openapi/salesforce-experience-cloud-rest-api-openapi.yml
  - openapi/salesforce-experience-cloud-sites-openapi.yml
  - openapi/salesforce-experience-cloud-templates-openapi.yml
  - openapi/salesforce-experience-cloud-user-interface-openapi.yml
  type: http
slug: salesforce-experience-cloud-authentication
source_filename: salesforce-experience-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-experience-cloud-cms-connect-openapi.yml, openapi/salesforce-experience-cloud-cms-delivery-openapi.yml,\n  openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml, openapi/salesforce-experience-cloud-connect-communities-openapi.yml,\n  openapi/salesforce-experience-cloud-graphql-openapi.yml, openapi/salesforce-experience-cloud-rest-api-openapi.yml,\n  openapi/salesforce-experience-cloud-sites-openapi.yml, openapi/salesforce-experience-cloud-templates-openapi.yml,\n  openapi/salesforce-experience-cloud-user-interface-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 2\n  description: Salesforce OAuth 2.0 authentication\n\
  \  sources:\n  - openapi/salesforce-experience-cloud-cms-connect-openapi.yml\n  - openapi/salesforce-experience-cloud-cms-delivery-openapi.yml\n  - openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml\n  - openapi/salesforce-experience-cloud-connect-communities-openapi.yml\n  - openapi/salesforce-experience-cloud-graphql-openapi.yml\n  - openapi/salesforce-experience-cloud-rest-api-openapi.yml\n  - openapi/salesforce-experience-cloud-sites-openapi.yml\n  - openapi/salesforce-experience-cloud-templates-openapi.yml\n  - openapi/salesforce-experience-cloud-user-interface-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  description: Bearer token obtained through OAuth 2.0 flow\n  sources:\n  - openapi/salesforce-experience-cloud-cms-connect-openapi.yml\n  - openapi/salesforce-experience-cloud-cms-delivery-openapi.yml\n  - openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml\n  - openapi/salesforce-experience-cloud-connect-communities-openapi.yml\n\
  \  - openapi/salesforce-experience-cloud-graphql-openapi.yml\n  - openapi/salesforce-experience-cloud-rest-api-openapi.yml\n  - openapi/salesforce-experience-cloud-sites-openapi.yml\n  - openapi/salesforce-experience-cloud-templates-openapi.yml\n  - openapi/salesforce-experience-cloud-user-interface-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/authentication/salesforce-experience-cloud-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
---
