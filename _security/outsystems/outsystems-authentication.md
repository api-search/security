---
api_key_in: []
api_specs:
- filename: outsystems-user-access-management-api-v1-openapi.json
  format: json
  label: OutSystems ODC User and Access Management API
  slug: user-access-management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-user-access-management-api-v1-openapi.json
- filename: outsystems-portfolio-api-v2-openapi.json
  format: json
  label: OutSystems ODC Portfolio API
  slug: portfolio-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-portfolio-api-v2-openapi.json
- filename: outsystems-portfolio-api-v1-openapi.json
  format: json
  label: OutSystems ODC Portfolio API (v1)
  slug: portfolio-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-portfolio-api-v1-openapi.json
- filename: outsystems-asset-repository-api-v1-openapi.json
  format: json
  label: OutSystems ODC Asset Repository API
  slug: asset-repository-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-asset-repository-api-v1-openapi.json
- filename: outsystems-asset-configurations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Asset Configurations API
  slug: asset-configurations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-asset-configurations-api-v1-openapi.json
- filename: outsystems-environment-configurations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Environment Configurations API
  slug: environment-configurations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-environment-configurations-api-v1-openapi.json
- filename: outsystems-build-operations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Build Operations API
  slug: build-operations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-build-operations-api-v1-openapi.json
- filename: outsystems-deployments-api-v1-openapi.json
  format: json
  label: OutSystems ODC Deployments API
  slug: deployments-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-deployments-api-v1-openapi.json
- filename: outsystems-dependency-management-api-v1-openapi.json
  format: json
  label: OutSystems ODC Dependency Management API
  slug: dependency-management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-dependency-management-api-v1-openapi.json
- filename: outsystems-code-quality-api-v1-openapi.json
  format: json
  label: OutSystems ODC Code Quality API
  slug: code-quality-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-code-quality-api-v1-openapi.json
- filename: outsystems-native-application-orchestration-service-api-v1-openapi.json
  format: json
  label: OutSystems ODC Native Mobile Build API
  slug: native-mobile-build-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-native-application-orchestration-service-api-v1-openapi.json
- filename: outsystems-external-library-generation-api-v1-openapi.json
  format: json
  label: OutSystems ODC External Library Generation API
  slug: external-library-generation-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-external-library-generation-api-v1-openapi.json
- filename: outsystems-subscription-api-v1-openapi.json
  format: json
  label: OutSystems ODC Subscription API
  slug: subscription-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-subscription-api-v1-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Outsystems Authentication
name_suffix: Authentication
oauth_flows: []
overview: OutSystems secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OutSystems
provider_slug: outsystems
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Enter your bearer token in the format 'Bearer {token}'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/outsystems-asset-configurations-api-v1-openapi.json
  - openapi/outsystems-asset-repository-api-v1-openapi.json
  - openapi/outsystems-build-operations-api-v1-openapi.json
  - openapi/outsystems-code-quality-api-v1-openapi.json
  - openapi/outsystems-dependency-management-api-v1-openapi.json
  - openapi/outsystems-deployments-api-v1-openapi.json
  - openapi/outsystems-environment-configurations-api-v1-openapi.json
  - openapi/outsystems-external-library-generation-api-v1-openapi.json
  - openapi/outsystems-native-application-orchestration-service-api-v1-openapi.json
  - openapi/outsystems-portfolio-api-v1-openapi.json
  - openapi/outsystems-portfolio-api-v2-openapi.json
  - openapi/outsystems-subscription-api-v1-openapi.json
  - openapi/outsystems-user-access-management-api-v1-openapi.json
  type: http
slug: outsystems-authentication
source_filename: outsystems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/outsystems-asset-configurations-api-v1-openapi.json, openapi/outsystems-asset-repository-api-v1-openapi.json,\n  openapi/outsystems-build-operations-api-v1-openapi.json, openapi/outsystems-code-quality-api-v1-openapi.json,\n  openapi/outsystems-dependency-management-api-v1-openapi.json, openapi/outsystems-deployments-api-v1-openapi.json,\n  openapi/outsystems-environment-configurations-api-v1-openapi.json, openapi/outsystems-external-library-generation-api-v1-openapi.json,\n  openapi/outsystems-native-application-orchestration-service-api-v1-openapi.json, openapi/outsystems-portfolio-api-v1-openapi.json,\n  openapi/outsystems-portfolio-api-v2-openapi.json, openapi/outsystems-subscription-api-v1-openapi.json\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Enter your bearer token in the format 'Bearer {token}'\n  sources:\n  - openapi/outsystems-asset-configurations-api-v1-openapi.json\n\
  \  - openapi/outsystems-asset-repository-api-v1-openapi.json\n  - openapi/outsystems-build-operations-api-v1-openapi.json\n  - openapi/outsystems-code-quality-api-v1-openapi.json\n  - openapi/outsystems-dependency-management-api-v1-openapi.json\n  - openapi/outsystems-deployments-api-v1-openapi.json\n  - openapi/outsystems-environment-configurations-api-v1-openapi.json\n  - openapi/outsystems-external-library-generation-api-v1-openapi.json\n  - openapi/outsystems-native-application-orchestration-service-api-v1-openapi.json\n  - openapi/outsystems-portfolio-api-v1-openapi.json\n  - openapi/outsystems-portfolio-api-v2-openapi.json\n  - openapi/outsystems-subscription-api-v1-openapi.json\n  - openapi/outsystems-user-access-management-api-v1-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/authentication/outsystems-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Low-Code
- Application Development
- Platform as a Service
- DevOps
- Deployment
- Identity and Access Management
- Artificial Intelligence
- Enterprise Software
- Mobile Development
---
