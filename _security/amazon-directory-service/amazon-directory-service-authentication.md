---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-directory-service-aws-directory-service-api-openapi.yml
  format: yaml
  label: Amazon Directory Service AWS Directory Service API
  slug: amazon-directory-service-aws-directory-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-aws-directory-service-api-openapi.yml
- filename: amazon-directory-service-ad-assessment-api-openapi.yml
  format: yaml
  label: Amazon Directory Service Directory Service Ad Assessment API
  slug: amazon-directory-service-ad-assessment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-ad-assessment-api-openapi.yml
- filename: amazon-directory-service-ca-enrollment-policy-api-openapi.yml
  format: yaml
  label: Amazon Directory Service Directory Service Ca Enrollment Policy API
  slug: amazon-directory-service-ca-enrollment-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-ca-enrollment-policy-api-openapi.yml
- filename: amazon-directory-service-directory-data-access-api-openapi.yml
  format: yaml
  label: Amazon Directory Service Directory Service Directory Data Access API
  slug: amazon-directory-service-directory-data-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-directory-data-access-api-openapi.yml
- filename: amazon-directory-service-operations-api-openapi.yml
  format: yaml
  label: Amazon Directory Service Directory Service Operations API
  slug: amazon-directory-service-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-operations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Directory Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Directory Service secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-directory-service-openapi.yaml
  type: apiKey
slug: amazon-directory-service-authentication
source_filename: amazon-directory-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-directory-service-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-directory-service-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/amazon-directory-service/authentication/amazon-directory-service-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Active Directory
- Authentication
- Directory Services
- Identity and Access Management
---
