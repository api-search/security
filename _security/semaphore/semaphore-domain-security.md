---
api_specs:
- filename: semaphore-dashboards-api-openapi.yml
  format: yaml
  label: Semaphore Dashboards API
  slug: semaphore-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-dashboards-api-openapi.yml
- filename: semaphore-deploymenttargets-api-openapi.yml
  format: yaml
  label: Semaphore DeploymentTargets API
  slug: semaphore-deploymenttargets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-deploymenttargets-api-openapi.yml
- filename: semaphore-notifications-api-openapi.yml
  format: yaml
  label: Semaphore Notifications API
  slug: semaphore-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-notifications-api-openapi.yml
- filename: semaphore-pipelines-api-openapi.yml
  format: yaml
  label: Semaphore Pipelines API
  slug: semaphore-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-pipelines-api-openapi.yml
- filename: semaphore-projects-api-openapi.yml
  format: yaml
  label: Semaphore Projects API
  slug: semaphore-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-projects-api-openapi.yml
- filename: semaphore-projectsecrets-api-openapi.yml
  format: yaml
  label: Semaphore ProjectSecrets API
  slug: semaphore-projectsecrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-projectsecrets-api-openapi.yml
- filename: semaphore-secrets-api-openapi.yml
  format: yaml
  label: Semaphore Secrets API
  slug: semaphore-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-secrets-api-openapi.yml
- filename: semaphore-selfhostedagents-api-openapi.yml
  format: yaml
  label: Semaphore SelfHostedAgents API
  slug: semaphore-selfhostedagents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-selfhostedagents-api-openapi.yml
- filename: semaphore-selfhostedagenttypes-api-openapi.yml
  format: yaml
  label: Semaphore SelfHostedAgentTypes API
  slug: semaphore-selfhostedagenttypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-selfhostedagenttypes-api-openapi.yml
- filename: semaphore-tasks-api-openapi.yml
  format: yaml
  label: Semaphore Tasks API
  slug: semaphore-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-tasks-api-openapi.yml
- filename: semaphore-workflows-api-openapi.yml
  format: yaml
  label: Semaphore Workflows API
  slug: semaphore-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: semaphore.io
  spf: true
hosts:
- cert_expires: Aug 31 11:03:05 2026 GMT
  host: semaphore.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Semaphore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Semaphore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Semaphore
provider_slug: semaphore
slug: semaphore-domain-security
source_filename: semaphore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: semaphore.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:03:05 2026 GMT\n  hsts: false\ndomains:\n- domain: semaphore.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/security/semaphore-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- Pipelines
- Workflows
- DevOps
- Build Automation
- Software Delivery
- Deployment
- Artifacts
---
