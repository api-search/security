---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-eks-clusters-api-openapi.yml
  format: yaml
  label: Amazon EKS Clusters API
  slug: amazon-eks-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-clusters-api-openapi.yml
- filename: amazon-eks-fargate-profiles-api-openapi.yml
  format: yaml
  label: Amazon EKS Fargate Profiles API
  slug: amazon-eks-fargate-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-fargate-profiles-api-openapi.yml
- filename: amazon-eks-node-groups-api-openapi.yml
  format: yaml
  label: Amazon EKS Node Groups API
  slug: amazon-eks-node-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-node-groups-api-openapi.yml
- filename: amazon-eks-add-ons-api-openapi.yml
  format: yaml
  label: Amazon EKS Add Ons API
  slug: amazon-eks-add-ons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-add-ons-api-openapi.yml
- filename: amazon-eks-access-entries-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Access Entries API
  slug: amazon-eks-access-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-access-entries-api-openapi.yml
- filename: amazon-eks-access-policies-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Access Policies API
  slug: amazon-eks-access-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-access-policies-api-openapi.yml
- filename: amazon-eks-capabilities-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Capabilities API
  slug: amazon-eks-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-capabilities-api-openapi.yml
- filename: amazon-eks-certificate-authorities-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Certificate Authorities API
  slug: amazon-eks-certificate-authorities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-certificate-authorities-api-openapi.yml
- filename: amazon-eks-eks-anywhere-subscriptions-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Eks Anywhere Subscriptions API
  slug: amazon-eks-eks-anywhere-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-eks-anywhere-subscriptions-api-openapi.yml
- filename: amazon-eks-identity-provider-configs-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Identity Provider Configs API
  slug: amazon-eks-identity-provider-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-identity-provider-configs-api-openapi.yml
- filename: amazon-eks-operations-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Operations API
  slug: amazon-eks-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-operations-api-openapi.yml
- filename: amazon-eks-pod-identity-associations-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Pod Identity Associations API
  slug: amazon-eks-pod-identity-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-pod-identity-associations-api-openapi.yml
- filename: amazon-eks-tags-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Tags API
  slug: amazon-eks-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-tags-api-openapi.yml
- filename: amazon-eks-updates-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Updates API
  slug: amazon-eks-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-updates-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon EKS Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EKS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EKS
provider_slug: amazon-eks
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-eks-access-entries-api-openapi.yml
  - openapi/amazon-eks-access-policies-api-openapi.yml
  - openapi/amazon-eks-add-ons-api-openapi.yml
  - openapi/amazon-eks-capabilities-api-openapi.yml
  - openapi/amazon-eks-certificate-authorities-api-openapi.yml
  - openapi/amazon-eks-clusters-api-openapi.yml
  - openapi/amazon-eks-eks-anywhere-subscriptions-api-openapi.yml
  - openapi/amazon-eks-fargate-profiles-api-openapi.yml
  - openapi/amazon-eks-identity-provider-configs-api-openapi.yml
  - openapi/amazon-eks-node-groups-api-openapi.yml
  - openapi/amazon-eks-operations-api-openapi.yml
  - openapi/amazon-eks-pod-identity-associations-api-openapi.yml
  - openapi/amazon-eks-tags-api-openapi.yml
  - openapi/amazon-eks-updates-api-openapi.yml
  type: apiKey
slug: amazon-eks-authentication
source_filename: amazon-eks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-eks-access-entries-api-openapi.yml, openapi/amazon-eks-access-policies-api-openapi.yml,\n  openapi/amazon-eks-add-ons-api-openapi.yml, openapi/amazon-eks-capabilities-api-openapi.yml,\n  openapi/amazon-eks-certificate-authorities-api-openapi.yml, openapi/amazon-eks-clusters-api-openapi.yml,\n  openapi/amazon-eks-eks-anywhere-subscriptions-api-openapi.yml, openapi/amazon-eks-fargate-profiles-api-openapi.yml,\n  openapi/amazon-eks-identity-provider-configs-api-openapi.yml, openapi/amazon-eks-node-groups-api-openapi.yml,\n  openapi/amazon-eks-operations-api-openapi.yml, openapi/amazon-eks-pod-identity-associations-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with\
  \ X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-eks-access-entries-api-openapi.yml\n  - openapi/amazon-eks-access-policies-api-openapi.yml\n  - openapi/amazon-eks-add-ons-api-openapi.yml\n  - openapi/amazon-eks-capabilities-api-openapi.yml\n  - openapi/amazon-eks-certificate-authorities-api-openapi.yml\n  - openapi/amazon-eks-clusters-api-openapi.yml\n  - openapi/amazon-eks-eks-anywhere-subscriptions-api-openapi.yml\n  - openapi/amazon-eks-fargate-profiles-api-openapi.yml\n  - openapi/amazon-eks-identity-provider-configs-api-openapi.yml\n  - openapi/amazon-eks-node-groups-api-openapi.yml\n  - openapi/amazon-eks-operations-api-openapi.yml\n  - openapi/amazon-eks-pod-identity-associations-api-openapi.yml\n  - openapi/amazon-eks-tags-api-openapi.yml\n  - openapi/amazon-eks-updates-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-eks/authentication/amazon-eks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Container Orchestration
- Containers
- EKS
- Kubernetes
---
