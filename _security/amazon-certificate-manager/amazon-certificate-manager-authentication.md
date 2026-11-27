---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-certificate-manager-certificates-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificates API
  slug: amazon-certificate-manager-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-certificates-api-openapi.yml
- filename: amazon-certificate-manager-acme-account-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Acme Account API
  slug: amazon-certificate-manager-acme-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-acme-account-api-openapi.yml
- filename: amazon-certificate-manager-acme-domain-validation-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Acme Domain Validation API
  slug: amazon-certificate-manager-acme-domain-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-acme-domain-validation-api-openapi.yml
- filename: amazon-certificate-manager-acme-endpoint-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Acme Endpoint API
  slug: amazon-certificate-manager-acme-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-acme-endpoint-api-openapi.yml
- filename: amazon-certificate-manager-acme-external-account-binding-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Acme External Account Binding API
  slug: amazon-certificate-manager-acme-external-account-binding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-acme-external-account-binding-api-openapi.yml
- filename: amazon-certificate-manager-operations-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Operations API
  slug: amazon-certificate-manager-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-operations-api-openapi.yml
- filename: amazon-certificate-manager-tag-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Tag API
  slug: amazon-certificate-manager-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-tag-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Certificate Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Certificate Manager secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Certificate Manager
provider_slug: amazon-certificate-manager
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-certificate-manager-acme-account-api-openapi.yml
  - openapi/amazon-certificate-manager-acme-domain-validation-api-openapi.yml
  - openapi/amazon-certificate-manager-acme-endpoint-api-openapi.yml
  - openapi/amazon-certificate-manager-acme-external-account-binding-api-openapi.yml
  - openapi/amazon-certificate-manager-certificates-api-openapi.yml
  - openapi/amazon-certificate-manager-operations-api-openapi.yml
  - openapi/amazon-certificate-manager-tag-api-openapi.yml
  type: apiKey
slug: amazon-certificate-manager-authentication
source_filename: amazon-certificate-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-certificate-manager-acme-account-api-openapi.yml, openapi/amazon-certificate-manager-acme-domain-validation-api-openapi.yml,\n  openapi/amazon-certificate-manager-acme-endpoint-api-openapi.yml, openapi/amazon-certificate-manager-acme-external-account-binding-api-openapi.yml,\n  openapi/amazon-certificate-manager-certificates-api-openapi.yml, openapi/amazon-certificate-manager-operations-api-openapi.yml,\n  openapi/amazon-certificate-manager-tag-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-certificate-manager-acme-account-api-openapi.yml\n \
  \ - openapi/amazon-certificate-manager-acme-domain-validation-api-openapi.yml\n  - openapi/amazon-certificate-manager-acme-endpoint-api-openapi.yml\n  - openapi/amazon-certificate-manager-acme-external-account-binding-api-openapi.yml\n  - openapi/amazon-certificate-manager-certificates-api-openapi.yml\n  - openapi/amazon-certificate-manager-operations-api-openapi.yml\n  - openapi/amazon-certificate-manager-tag-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-certificate-manager/authentication/amazon-certificate-manager-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Certificates
- Encryption
- Security
- SSL
- TLS
---
