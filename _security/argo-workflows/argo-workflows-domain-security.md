---
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
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: argo-workflows.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argo Workflows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argo Workflows, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Argo Workflows
provider_slug: argo-workflows
slug: argo-workflows-domain-security
source_filename: argo-workflows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: argo-workflows.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/security/argo-workflows-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine-Learning
- Open-Source
- Workflow Engine
---
