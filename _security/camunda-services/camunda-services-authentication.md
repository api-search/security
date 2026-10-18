---
anonymous_access: false
api_key_in: []
api_specs:
- filename: camunda-services-actuator-api-openapi.yml
  format: yaml
  label: Camunda Services Actuator API
  slug: camunda-services-actuator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-actuator-api-openapi.yml
- filename: camunda-services-auth-api-openapi.yml
  format: yaml
  label: Camunda Services Auth API
  slug: camunda-services-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-auth-api-openapi.yml
- filename: camunda-services-camunda-services-api-api-openapi.yml
  format: yaml
  label: Camunda Services Camunda Services API
  slug: camunda-services-camunda-services-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-camunda-services-api-api-openapi.yml
- filename: camunda-services-cluster-api-openapi.yml
  format: yaml
  label: Camunda Services Cluster API
  slug: camunda-services-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-cluster-api-openapi.yml
- filename: camunda-services-cluster-id-api-openapi.yml
  format: yaml
  label: Camunda Services Cluster Id API
  slug: camunda-services-cluster-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-cluster-id-api-openapi.yml
- filename: camunda-services-deployments-api-openapi.yml
  format: yaml
  label: Camunda Services Deployments API
  slug: camunda-services-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-deployments-api-openapi.yml
- filename: camunda-services-info-api-openapi.yml
  format: yaml
  label: Camunda Services Info API
  slug: camunda-services-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-info-api-openapi.yml
- filename: camunda-services-ingestion-api-openapi.yml
  format: yaml
  label: Camunda Services Ingestion API
  slug: camunda-services-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-ingestion-api-openapi.yml
- filename: camunda-services-members-api-openapi.yml
  format: yaml
  label: Camunda Services Members API
  slug: camunda-services-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-members-api-openapi.yml
- filename: camunda-services-process-definitions-api-openapi.yml
  format: yaml
  label: Camunda Services Process Definitions API
  slug: camunda-services-process-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-process-definitions-api-openapi.yml
- filename: camunda-services-process-instances-api-openapi.yml
  format: yaml
  label: Camunda Services Process Instances API
  slug: camunda-services-process-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-process-instances-api-openapi.yml
- filename: camunda-services-public-api-openapi.yml
  format: yaml
  label: Camunda Services Public API
  slug: camunda-services-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-public-api-openapi.yml
- filename: camunda-services-readyz-api-openapi.yml
  format: yaml
  label: Camunda Services Readyz API
  slug: camunda-services-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-readyz-api-openapi.yml
- filename: camunda-services-resources-api-openapi.yml
  format: yaml
  label: Camunda Services Resources API
  slug: camunda-services-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-resources-api-openapi.yml
- filename: camunda-services-setup-api-openapi.yml
  format: yaml
  label: Camunda Services Setup API
  slug: camunda-services-setup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-setup-api-openapi.yml
- filename: camunda-services-topology-api-openapi.yml
  format: yaml
  label: Camunda Services Topology API
  slug: camunda-services-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-topology-api-openapi.yml
- filename: camunda-services-user-tasks-api-openapi.yml
  format: yaml
  label: Camunda Services User Tasks API
  slug: camunda-services-user-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-user-tasks-api-openapi.yml
- filename: camunda-services-chat-completions-api-openapi.yml
  format: yaml
  label: Camunda Services Chat Completions API
  slug: camunda-services-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/camunda-services-chat-completions-api-openapi.yml
auth_types: []
description: Camunda Services authentication methods for the Orchestration Cluster
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Camunda Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: Camunda Services declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Camunda Services
provider_slug: camunda-services
scheme_count: 2
schemes:
- evidence: With Basic authentication, Orchestration Cluster components are protected with a username and password.
  name: Basic authentication
  type: http-basic
- evidence: With OIDC, authentication is delegated to an external Identity Provider (IdP) using OpenID Connect (OIDC).
  name: OIDC
  type: oauth2
slug: camunda-services-authentication
source_filename: camunda-services-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.camunda.io/docs/self-managed/concepts/authentication/authentication-to-orchestration-cluster/
source_yaml: "generated: '2026-10-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.camunda.io/docs/self-managed/concepts/authentication/authentication-to-orchestration-cluster/\nsources:\n- https://docs.camunda.io/docs/self-managed/concepts/authentication/authentication-to-orchestration-cluster/\n- https://docs.camunda.io/docs/reference/glossary/\n- https://docs.camunda.io/docs/guides/getting-started-agentic-orchestration/\n- https://docs.camunda.io/docs/next/guides/getting-started-agentic-orchestration/\ndescription: Camunda Services authentication methods for the Orchestration Cluster\nschemes:\n- type: http-basic\n  name: Basic authentication\n  evidence: With Basic authentication, Orchestration Cluster components are protected with a username and password.\n- type: oauth2\n  name: OIDC\n  evidence: With OIDC, authentication is delegated to an external Identity Provider (IdP) using OpenID Connect (OIDC).\ndocs: https://docs.camunda.io/docs/self-managed/concepts/authentication/authentication-to-orchestration-cluster/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/authentication/camunda-services-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Workflows
- BPMN
- DMN
- Automation
---
