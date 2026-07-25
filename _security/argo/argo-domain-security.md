---
api_specs:
- filename: argo-events-asyncapi.yml
  format: yaml
  label: Argo Events API
  slug: argo-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/asyncapi/argo-events-asyncapi.yml
- filename: argo-applications-api-openapi.yml
  format: yaml
  label: Argo Applications API
  slug: argo-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-applications-api-openapi.yml
- filename: argo-clusters-api-openapi.yml
  format: yaml
  label: Argo Clusters API
  slug: argo-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-clusters-api-openapi.yml
- filename: argo-cron-workflows-api-openapi.yml
  format: yaml
  label: Argo Cron Workflows API
  slug: argo-cron-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-cron-workflows-api-openapi.yml
- filename: argo-info-api-openapi.yml
  format: yaml
  label: Argo Info API
  slug: argo-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-info-api-openapi.yml
- filename: argo-projects-api-openapi.yml
  format: yaml
  label: Argo Projects API
  slug: argo-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-projects-api-openapi.yml
- filename: argo-repositories-api-openapi.yml
  format: yaml
  label: Argo Repositories API
  slug: argo-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-repositories-api-openapi.yml
- filename: argo-session-api-openapi.yml
  format: yaml
  label: Argo Session API
  slug: argo-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-session-api-openapi.yml
- filename: argo-settings-api-openapi.yml
  format: yaml
  label: Argo Settings API
  slug: argo-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-settings-api-openapi.yml
- filename: argo-version-api-openapi.yml
  format: yaml
  label: Argo Version API
  slug: argo-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-version-api-openapi.yml
- filename: argo-workflow-archives-api-openapi.yml
  format: yaml
  label: Argo Workflow Archives API
  slug: argo-workflow-archives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-workflow-archives-api-openapi.yml
- filename: argo-workflow-templates-api-openapi.yml
  format: yaml
  label: Argo Workflow Templates API
  slug: argo-workflow-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-workflow-templates-api-openapi.yml
- filename: argo-workflows-api-openapi.yml
  format: yaml
  label: Argo Workflows API
  slug: argo-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/openapi/argo-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
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
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: argo-cd.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: argo-rollouts.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Argo
provider_slug: argo
slug: argo-domain-security
source_filename: argo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: argo-workflows.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: argo-cd.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: argo-rollouts.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/security/argo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
---
