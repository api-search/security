---
api_specs:
- filename: circleci-runner-api-openapi.yml
  format: yaml
  label: CircleCI Self-Hosted Runner API
  slug: runner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-runner-api-openapi.yml
- filename: circleci-webhooks-asyncapi.yml
  format: yaml
  label: CircleCI Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/asyncapi/circleci-webhooks-asyncapi.yml
- filename: circleci-artifact-api-openapi.yml
  format: yaml
  label: CircleCI Artifact API
  slug: circleci-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-artifact-api-openapi.yml
- filename: circleci-build-api-openapi.yml
  format: yaml
  label: CircleCI Build API
  slug: circleci-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-build-api-openapi.yml
- filename: circleci-context-api-openapi.yml
  format: yaml
  label: CircleCI Context API
  slug: circleci-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-context-api-openapi.yml
- filename: circleci-insights-api-openapi.yml
  format: yaml
  label: CircleCI Insights API
  slug: circleci-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-insights-api-openapi.yml
- filename: circleci-job-api-openapi.yml
  format: yaml
  label: CircleCI Job API
  slug: circleci-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-job-api-openapi.yml
- filename: circleci-pipeline-api-openapi.yml
  format: yaml
  label: CircleCI Pipeline API
  slug: circleci-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-pipeline-api-openapi.yml
- filename: circleci-project-api-openapi.yml
  format: yaml
  label: CircleCI Project API
  slug: circleci-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-project-api-openapi.yml
- filename: circleci-resource-class-api-openapi.yml
  format: yaml
  label: CircleCI Resource Class API
  slug: circleci-resource-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-resource-class-api-openapi.yml
- filename: circleci-runner-task-api-openapi.yml
  format: yaml
  label: CircleCI Runner Task API
  slug: circleci-runner-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-runner-task-api-openapi.yml
- filename: circleci-schedule-api-openapi.yml
  format: yaml
  label: CircleCI Schedule API
  slug: circleci-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-schedule-api-openapi.yml
- filename: circleci-ssh-key-api-openapi.yml
  format: yaml
  label: CircleCI SSH Key API
  slug: circleci-ssh-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-ssh-key-api-openapi.yml
- filename: circleci-test-metadata-api-openapi.yml
  format: yaml
  label: CircleCI Test Metadata API
  slug: circleci-test-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-test-metadata-api-openapi.yml
- filename: circleci-user-api-openapi.yml
  format: yaml
  label: CircleCI User API
  slug: circleci-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-user-api-openapi.yml
- filename: circleci-webhook-api-openapi.yml
  format: yaml
  label: CircleCI Webhook API
  slug: circleci-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-webhook-api-openapi.yml
- filename: circleci-workflow-api-openapi.yml
  format: yaml
  label: CircleCI Workflow API
  slug: circleci-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/openapi/circleci-workflow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: circleci.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: circleci.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: runner.circleci.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circleci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CircleCI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CircleCI
provider_slug: circleci
slug: circleci-domain-security
source_filename: circleci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circleci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: runner.circleci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: circleci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circleci/refs/heads/main/security/circleci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
---
