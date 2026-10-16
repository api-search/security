---
anonymous_access: false
api_key_in: []
api_specs:
- filename: camunda-services-apis-tools-openapi-generated.yml
  format: yaml
  label: Camunda Services apis tools API
  slug: apis-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/_ae-authored/camunda-services-apis-tools-openapi-generated.yml
- filename: camunda-services-core-openapi-generated.yml
  format: yaml
  label: Camunda Services core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/_ae-authored/camunda-services-core-openapi-generated.yml
- filename: camunda-services-self-managed-openapi-generated.yml
  format: yaml
  label: Camunda Services self managed API
  slug: self-managed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/_ae-authored/camunda-services-self-managed-openapi-generated.yml
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
- Workflow
- BPMN
- DMN
- Automation
---
