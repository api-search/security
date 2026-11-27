---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-workmail-amazon-workmail-api-openapi.yml
  format: yaml
  label: Amazon WorkMail Amazon WorkMail API
  slug: amazon-workmail-amazon-workmail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workmail/openapi/amazon-workmail-amazon-workmail-api-openapi.yml
- filename: amazon-workmail-identity-provider-configuration-api-openapi.yml
  format: yaml
  label: Amazon WorkMail Workmail Identity Provider Configuration API
  slug: amazon-workmail-identity-provider-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workmail/openapi/amazon-workmail-identity-provider-configuration-api-openapi.yml
- filename: amazon-workmail-operations-api-openapi.yml
  format: yaml
  label: Amazon WorkMail Workmail Operations API
  slug: amazon-workmail-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workmail/openapi/amazon-workmail-operations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon WorkMail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon WorkMail secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-workmail-amazon-workmail-api-openapi.yml
  - openapi/amazon-workmail-identity-provider-configuration-api-openapi.yml
  - openapi/amazon-workmail-operations-api-openapi.yml
  type: apiKey
slug: amazon-workmail-authentication
source_filename: amazon-workmail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-workmail-amazon-workmail-api-openapi.yml, openapi/amazon-workmail-identity-provider-configuration-api-openapi.yml,\n  openapi/amazon-workmail-operations-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-workmail-amazon-workmail-api-openapi.yml\n  - openapi/amazon-workmail-identity-provider-configuration-api-openapi.yml\n  - openapi/amazon-workmail-operations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-workmail/authentication/amazon-workmail-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Business Communication
- Calendar
- Email
- Enterprise
---
