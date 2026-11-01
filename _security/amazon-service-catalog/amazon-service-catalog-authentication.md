---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-service-catalog-portfolios-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Portfolios API
  slug: amazon-service-catalog-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-portfolios-api-openapi.yml
- filename: amazon-service-catalog-products-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Products API
  slug: amazon-service-catalog-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-products-api-openapi.yml
- filename: amazon-service-catalog-provisioned-products-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Provisioned Products API
  slug: amazon-service-catalog-provisioned-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-provisioned-products-api-openapi.yml
- filename: amazon-service-catalog-budget-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Budget API
  slug: amazon-service-catalog-budget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-budget-api-openapi.yml
- filename: amazon-service-catalog-constraint-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Constraint API
  slug: amazon-service-catalog-constraint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-constraint-api-openapi.yml
- filename: amazon-service-catalog-operations-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Operations API
  slug: amazon-service-catalog-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-operations-api-openapi.yml
- filename: amazon-service-catalog-portfolio-share-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Portfolio Share API
  slug: amazon-service-catalog-portfolio-share-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-portfolio-share-api-openapi.yml
- filename: amazon-service-catalog-principal-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Principal API
  slug: amazon-service-catalog-principal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-principal-api-openapi.yml
- filename: amazon-service-catalog-provisioned-product-plan-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Provisioned Product Plan API
  slug: amazon-service-catalog-provisioned-product-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-provisioned-product-plan-api-openapi.yml
- filename: amazon-service-catalog-provisioning-artifact-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Provisioning Artifact API
  slug: amazon-service-catalog-provisioning-artifact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-provisioning-artifact-api-openapi.yml
- filename: amazon-service-catalog-service-action-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Service Action API
  slug: amazon-service-catalog-service-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-service-action-api-openapi.yml
- filename: amazon-service-catalog-tag-option-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Tag Option API
  slug: amazon-service-catalog-tag-option-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-tag-option-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Service Catalog Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Service Catalog secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Service Catalog
provider_slug: amazon-service-catalog
scheme_count: 1
schemes:
- description: AWS Signature Version 4 authentication
  in: header
  name: AWSSignatureV4
  parameter: Authorization
  sources:
  - openapi/amazon-service-catalog-openapi.yml
  type: apiKey
slug: amazon-service-catalog-authentication
source_filename: amazon-service-catalog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-service-catalog-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AWSSignatureV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication\n  sources:\n  - openapi/amazon-service-catalog-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-service-catalog/authentication/amazon-service-catalog-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Governance
- Compliance
- IT Governance
- Service Catalog
---
