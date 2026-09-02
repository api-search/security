---
api_key_in:
- header
api_specs:
- filename: vellum-default-api-openapi.yml
  format: yaml
  label: Vellum AI Default API
  slug: vellum-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-default-api-openapi.yml
- filename: vellum-subpackage-deployments-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_deployments API
  slug: vellum-subpackage-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-deployments-api-openapi.yml
- filename: vellum-subpackage-documentindexes-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_documentIndexes API
  slug: vellum-subpackage-documentindexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-documentindexes-api-openapi.yml
- filename: vellum-subpackage-documents-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_documents API
  slug: vellum-subpackage-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-documents-api-openapi.yml
- filename: vellum-subpackage-events-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_events API
  slug: vellum-subpackage-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-events-api-openapi.yml
- filename: vellum-subpackage-folderentities-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_folderEntities API
  slug: vellum-subpackage-folderentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-folderentities-api-openapi.yml
- filename: vellum-subpackage-sandboxes-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_sandboxes API
  slug: vellum-subpackage-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-sandboxes-api-openapi.yml
- filename: vellum-subpackage-testsuiteruns-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_testSuiteRuns API
  slug: vellum-subpackage-testsuiteruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-testsuiteruns-api-openapi.yml
- filename: vellum-subpackage-testsuites-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_testSuites API
  slug: vellum-subpackage-testsuites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-testsuites-api-openapi.yml
- filename: vellum-subpackage-uploadedfiles-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_uploadedFiles API
  slug: vellum-subpackage-uploadedfiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-uploadedfiles-api-openapi.yml
- filename: vellum-subpackage-workflowdeployments-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_workflowDeployments API
  slug: vellum-subpackage-workflowdeployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-workflowdeployments-api-openapi.yml
- filename: vellum-subpackage-workflowexecutions-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_workflowExecutions API
  slug: vellum-subpackage-workflowexecutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-workflowexecutions-api-openapi.yml
- filename: vellum-subpackage-workflows-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_workflows API
  slug: vellum-subpackage-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-workflows-api-openapi.yml
- filename: vellum-subpackage-workflowsandboxes-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_workflowSandboxes API
  slug: vellum-subpackage-workflowsandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-workflowsandboxes-api-openapi.yml
- filename: vellum-subpackage-workspacesecrets-api-openapi.yml
  format: yaml
  label: Vellum AI subpackage_workspaceSecrets API
  slug: vellum-subpackage-workspacesecrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/openapi/vellum-subpackage-workspacesecrets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vellum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vellum AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vellum AI
provider_slug: vellum
scheme_count: 1
schemes:
- in: header
  name: default
  parameter: X-API-KEY
  sources:
  - openapi/vellum-openapi.json
  type: apiKey
slug: vellum-authentication
source_filename: vellum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vellum-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: default\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/vellum-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vellum/refs/heads/main/authentication/vellum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- LLM Platform
- Prompt Engineering
- Workflows
- Evaluations
- LLMOps
- RAG
- Observability
- Datasets
- Deployment
- Multi-Provider
- Agent Builder
- Self-Hosted
---
