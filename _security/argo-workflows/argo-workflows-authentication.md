---
api_key_in:
- header
api_specs:
- filename: argo-workflows-archivedworkflowservice-api-openapi.yml
  format: yaml
  label: Argo Workflows ArchivedWorkflowService API
  slug: argo-workflows-archivedworkflowservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-archivedworkflowservice-api-openapi.yml
- filename: argo-workflows-artifactservice-api-openapi.yml
  format: yaml
  label: Argo Workflows ArtifactService API
  slug: argo-workflows-artifactservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-artifactservice-api-openapi.yml
- filename: argo-workflows-clusterworkflowtemplateservice-api-openapi.yml
  format: yaml
  label: Argo Workflows ClusterWorkflowTemplateService API
  slug: argo-workflows-clusterworkflowtemplateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-clusterworkflowtemplateservice-api-openapi.yml
- filename: argo-workflows-cronworkflowservice-api-openapi.yml
  format: yaml
  label: Argo Workflows CronWorkflowService API
  slug: argo-workflows-cronworkflowservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-cronworkflowservice-api-openapi.yml
- filename: argo-workflows-eventservice-api-openapi.yml
  format: yaml
  label: Argo Workflows EventService API
  slug: argo-workflows-eventservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-eventservice-api-openapi.yml
- filename: argo-workflows-eventsourceservice-api-openapi.yml
  format: yaml
  label: Argo Workflows EventSourceService API
  slug: argo-workflows-eventsourceservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-eventsourceservice-api-openapi.yml
- filename: argo-workflows-infoservice-api-openapi.yml
  format: yaml
  label: Argo Workflows InfoService API
  slug: argo-workflows-infoservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-infoservice-api-openapi.yml
- filename: argo-workflows-sensorservice-api-openapi.yml
  format: yaml
  label: Argo Workflows SensorService API
  slug: argo-workflows-sensorservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-sensorservice-api-openapi.yml
- filename: argo-workflows-syncservice-api-openapi.yml
  format: yaml
  label: Argo Workflows SyncService API
  slug: argo-workflows-syncservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-syncservice-api-openapi.yml
- filename: argo-workflows-workflowservice-api-openapi.yml
  format: yaml
  label: Argo Workflows WorkflowService API
  slug: argo-workflows-workflowservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-workflowservice-api-openapi.yml
- filename: argo-workflows-workflowtemplateservice-api-openapi.yml
  format: yaml
  label: Argo Workflows WorkflowTemplateService API
  slug: argo-workflows-workflowtemplateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/openapi/argo-workflows-workflowtemplateservice-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Argo Workflows Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argo Workflows secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argo Workflows
provider_slug: argo-workflows
scheme_count: 1
schemes:
- description: JWT Bearer token
  in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/argo-workflows-openapi.json
  type: apiKey
slug: argo-workflows-authentication
source_filename: argo-workflows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/argo-workflows-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT Bearer token\n  sources:\n  - openapi/argo-workflows-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/authentication/argo-workflows-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine-Learning
- Open-Source
- Workflow Engine
---
