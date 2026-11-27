---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-private-ca-aws-certificate-manager-private-certificate-authority-api-openapi.yml
  format: yaml
  label: Amazon Private CA AWS Certificate Manager Private Certificate Authority API
  slug: amazon-private-ca-aws-certificate-manager-private-certificate-authority-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-private-ca/openapi/amazon-private-ca-aws-certificate-manager-private-certificate-authority-api-openapi.yml
- filename: amazon-private-ca-accesscontrolentries-api-openapi.yml
  format: yaml
  label: Amazon Private CA Private Ca Accesscontrolentries API
  slug: amazon-private-ca-accesscontrolentries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-private-ca/openapi/amazon-private-ca-accesscontrolentries-api-openapi.yml
- filename: amazon-private-ca-connectors-api-openapi.yml
  format: yaml
  label: Amazon Private CA Private Ca Connectors API
  slug: amazon-private-ca-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-private-ca/openapi/amazon-private-ca-connectors-api-openapi.yml
- filename: amazon-private-ca-directoryregistrations-api-openapi.yml
  format: yaml
  label: Amazon Private CA Private Ca Directoryregistrations API
  slug: amazon-private-ca-directoryregistrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-private-ca/openapi/amazon-private-ca-directoryregistrations-api-openapi.yml
- filename: amazon-private-ca-operations-api-openapi.yml
  format: yaml
  label: Amazon Private CA Private Ca Operations API
  slug: amazon-private-ca-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-private-ca/openapi/amazon-private-ca-operations-api-openapi.yml
- filename: amazon-private-ca-serviceprincipalnames-api-openapi.yml
  format: yaml
  label: Amazon Private CA Private Ca Serviceprincipalnames API
  slug: amazon-private-ca-serviceprincipalnames-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-private-ca/openapi/amazon-private-ca-serviceprincipalnames-api-openapi.yml
- filename: amazon-private-ca-tags-api-openapi.yml
  format: yaml
  label: Amazon Private CA Private Ca Tags API
  slug: amazon-private-ca-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-private-ca/openapi/amazon-private-ca-tags-api-openapi.yml
- filename: amazon-private-ca-templates-api-openapi.yml
  format: yaml
  label: Amazon Private CA Private Ca Templates API
  slug: amazon-private-ca-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-private-ca/openapi/amazon-private-ca-templates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Private CA Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Private CA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-private-ca-openapi-original.yaml
  type: apiKey
slug: amazon-private-ca-authentication
source_filename: amazon-private-ca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-private-ca-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-private-ca-openapi-original.yaml\n"
source_yaml_url: https://artifacts.apis.io/amazon-private-ca/authentication/amazon-private-ca-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
---
