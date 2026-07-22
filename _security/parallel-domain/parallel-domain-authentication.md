---
api_key_in:
- environment
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Parallel Domain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parallel Domain secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Parallel Domain
provider_slug: parallel-domain
scheme_count: 3
schemes:
- description: Organization Step API key used by the SDK to authenticate Data Lab generation requests.
  env: PD_CLIENT_STEP_API_KEY_ENV
  in: environment
  name: StepApiKey
  sources:
  - https://parallel-domain.github.io/pd-sdk/
  type: apiKey
- description: Organization identifier scoping requests to the caller's Parallel Domain org.
  env: PD_CLIENT_ORG_ENV
  in: environment
  name: ClientOrg
  sources:
  - https://parallel-domain.github.io/pd-sdk/
  type: apiKey
- description: Path to a client credentials file consumed by the SDK.
  env: PD_CLIENT_CREDENTIALS_PATH_ENV
  in: environment
  name: ClientCredentialsFile
  sources:
  - https://parallel-domain.github.io/pd-sdk/
  type: apiKey
slug: parallel-domain-authentication
source_filename: parallel-domain-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://parallel-domain.github.io/pd-sdk/\ndocs: https://parallel-domain.github.io/pd-sdk/\nnotes: >-\n  Parallel Domain has no public REST/OpenAPI surface; access is through the\n  first-party Python SDK (paralleldomain / pd-sdk) and the app console at\n  app.paralleldomain.com. The SDK authenticates to the Data Lab / Step\n  generation backend with an organization-scoped API key plus a credentials\n  file, configured through environment variables. Auth model derived from the\n  SDK getting-started docs, not from a machine-readable spec.\nsummary:\n  types: [apiKey]\n  api_key_in: [environment]\n  oauth2_flows: []\nschemes:\n- name: StepApiKey\n  type: apiKey\n  in: environment\n  env: PD_CLIENT_STEP_API_KEY_ENV\n  description: Organization Step API key used by the SDK to authenticate Data Lab generation requests.\n  sources: [https://parallel-domain.github.io/pd-sdk/]\n- name: ClientOrg\n  type: apiKey\n  in: environment\n\
  \  env: PD_CLIENT_ORG_ENV\n  description: Organization identifier scoping requests to the caller's Parallel Domain org.\n  sources: [https://parallel-domain.github.io/pd-sdk/]\n- name: ClientCredentialsFile\n  type: apiKey\n  in: environment\n  env: PD_CLIENT_CREDENTIALS_PATH_ENV\n  description: Path to a client credentials file consumed by the SDK.\n  sources: [https://parallel-domain.github.io/pd-sdk/]\nconsole: https://app.paralleldomain.com/auth/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel-domain/refs/heads/main/authentication/parallel-domain-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Ai
- Synthetic Data
- Simulation
- Autonomous Vehicles
- Computer Vision
- Machine Learning
- Robotics
- SDK
---
