---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ubicloud-audit-log-api-openapi.yml
  format: yaml
  label: Ubicloud Audit Log API
  slug: ubicloud-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-audit-log-api-openapi.yml
- filename: ubicloud-firewall-api-openapi.yml
  format: yaml
  label: Ubicloud Firewall API
  slug: ubicloud-firewall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-firewall-api-openapi.yml
- filename: ubicloud-firewall-rule-api-openapi.yml
  format: yaml
  label: Ubicloud Firewall Rule API
  slug: ubicloud-firewall-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-firewall-rule-api-openapi.yml
- filename: ubicloud-github-api-openapi.yml
  format: yaml
  label: Ubicloud GitHub API
  slug: ubicloud-github-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-github-api-openapi.yml
- filename: ubicloud-inference-api-key-api-openapi.yml
  format: yaml
  label: Ubicloud Inference Api Key API
  slug: ubicloud-inference-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-inference-api-key-api-openapi.yml
- filename: ubicloud-inference-endpoint-api-openapi.yml
  format: yaml
  label: Ubicloud Inference Endpoint API
  slug: ubicloud-inference-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-inference-endpoint-api-openapi.yml
- filename: ubicloud-kubernetes-cluster-api-openapi.yml
  format: yaml
  label: Ubicloud Kubernetes Cluster API
  slug: ubicloud-kubernetes-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-kubernetes-cluster-api-openapi.yml
- filename: ubicloud-load-balancer-api-openapi.yml
  format: yaml
  label: Ubicloud Load Balancer API
  slug: ubicloud-load-balancer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-load-balancer-api-openapi.yml
- filename: ubicloud-machine-image-api-openapi.yml
  format: yaml
  label: Ubicloud Machine Image API
  slug: ubicloud-machine-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-machine-image-api-openapi.yml
- filename: ubicloud-postgres-database-api-openapi.yml
  format: yaml
  label: Ubicloud Postgres Database API
  slug: ubicloud-postgres-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-postgres-database-api-openapi.yml
- filename: ubicloud-postgres-firewall-rule-api-openapi.yml
  format: yaml
  label: Ubicloud Postgres Firewall Rule API
  slug: ubicloud-postgres-firewall-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-postgres-firewall-rule-api-openapi.yml
- filename: ubicloud-postgres-log-destination-api-openapi.yml
  format: yaml
  label: Ubicloud Postgres Log Destination API
  slug: ubicloud-postgres-log-destination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-postgres-log-destination-api-openapi.yml
- filename: ubicloud-postgres-metric-destination-api-openapi.yml
  format: yaml
  label: Ubicloud Postgres Metric Destination API
  slug: ubicloud-postgres-metric-destination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-postgres-metric-destination-api-openapi.yml
- filename: ubicloud-private-location-api-openapi.yml
  format: yaml
  label: Ubicloud Private Location API
  slug: ubicloud-private-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-private-location-api-openapi.yml
- filename: ubicloud-private-subnet-api-openapi.yml
  format: yaml
  label: Ubicloud Private Subnet API
  slug: ubicloud-private-subnet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-private-subnet-api-openapi.yml
- filename: ubicloud-project-api-openapi.yml
  format: yaml
  label: Ubicloud Project API
  slug: ubicloud-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-project-api-openapi.yml
- filename: ubicloud-ssh-public-key-api-openapi.yml
  format: yaml
  label: Ubicloud SSH Public Key API
  slug: ubicloud-ssh-public-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-ssh-public-key-api-openapi.yml
- filename: ubicloud-virtual-machine-api-openapi.yml
  format: yaml
  label: Ubicloud Virtual Machine API
  slug: ubicloud-virtual-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/openapi/ubicloud-virtual-machine-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ubicloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ubicloud secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ubicloud
provider_slug: ubicloud
scheme_count: 1
schemes:
- bearerFormat: JWT
  credential: personal access token
  evidence: The Ubicloud API uses personal access tokens for authentication.
  header: Authorization
  in: header
  invalid_token_status: 419
  name: BearerAuth
  obtain: Create Token button on the project Tokens page in the console
  scheme: bearer
  sources:
  - openapi/ubicloud-openapi.yml
  type: http
slug: ubicloud-authentication
source_filename: ubicloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://www.ubicloud.com/docs/api-reference/overview\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ubicloud-openapi.yml\n  credential: personal access token\n  obtain: Create Token button on the project Tokens page in the console\n  in: header\n  header: Authorization\n  evidence: The Ubicloud API uses personal access tokens for authentication.\n  invalid_token_status: 419\ndocs: https://www.ubicloud.com/docs/api-reference/overview\nother_credentials:\n- name: Inference API key\n  docs: https://www.ubicloud.com/docs/inference/api-key\n  note: Separate keys for the AI inference endpoints, managed via the inference-api-key\n    operations.\n- name: CLI\n  note: ubi reads the personal access token from the UBI_TOKEN environment variable.\nauthorization:\n  model: attribute-based access control (ABAC) per project\n  docs: https://www.ubicloud.com/docs/security/authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubicloud/refs/heads/main/authentication/ubicloud-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cloud Computing
- Open Source
- Infrastructure as a Service
- PostgreSQL
- Kubernetes
- Virtual Machines
- GitHub Actions
---
