---
api_key_in: []
api_specs:
- filename: employment-hero-bank-accounts-api-openapi.yml
  format: yaml
  label: Employment Hero Bank Accounts API
  slug: employment-hero-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-bank-accounts-api-openapi.yml
- filename: employment-hero-certifications-api-openapi.yml
  format: yaml
  label: Employment Hero Certifications API
  slug: employment-hero-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-certifications-api-openapi.yml
- filename: employment-hero-cost-centres-api-openapi.yml
  format: yaml
  label: Employment Hero Cost Centres API
  slug: employment-hero-cost-centres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-cost-centres-api-openapi.yml
- filename: employment-hero-custom-fields-api-openapi.yml
  format: yaml
  label: Employment Hero Custom Fields API
  slug: employment-hero-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-custom-fields-api-openapi.yml
- filename: employment-hero-departments-api-openapi.yml
  format: yaml
  label: Employment Hero Departments API
  slug: employment-hero-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-departments-api-openapi.yml
- filename: employment-hero-documents-api-openapi.yml
  format: yaml
  label: Employment Hero Documents API
  slug: employment-hero-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-documents-api-openapi.yml
- filename: employment-hero-emergency-contacts-api-openapi.yml
  format: yaml
  label: Employment Hero Emergency Contacts API
  slug: employment-hero-emergency-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-emergency-contacts-api-openapi.yml
- filename: employment-hero-employees-api-openapi.yml
  format: yaml
  label: Employment Hero Employees API
  slug: employment-hero-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-employees-api-openapi.yml
- filename: employment-hero-forms-api-openapi.yml
  format: yaml
  label: Employment Hero Forms API
  slug: employment-hero-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-forms-api-openapi.yml
- filename: employment-hero-job-histories-api-openapi.yml
  format: yaml
  label: Employment Hero Job Histories API
  slug: employment-hero-job-histories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/openapi/employment-hero-job-histories-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Employment Hero Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Employment Hero secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Employment Hero
provider_slug: employment-hero
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://oauth.employmenthero.com/oauth2/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://oauth.employmenthero.com/oauth2/token
  name: oauth2
  sources:
  - openapi/employment-hero-openapi.yml
  type: oauth2
slug: employment-hero-authentication
source_filename: employment-hero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/employment-hero-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.employmenthero.com/oauth2/authorize\n    tokenUrl: https://oauth.employmenthero.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/employment-hero-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/authentication/employment-hero-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HR
- HRIS
- Payroll
- Recruitment
- Employee Benefits
- Workforce Management
- HR Tech
---
