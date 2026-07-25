---
api_specs:
- filename: figure-eight-account-info-api-openapi.yml
  format: yaml
  label: Figure Eight Account Info API
  slug: figure-eight-account-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-account-info-api-openapi.yml
- filename: figure-eight-job-create-update-api-openapi.yml
  format: yaml
  label: Figure Eight Job Create/Update API
  slug: figure-eight-job-create-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-job-create-update-api-openapi.yml
- filename: figure-eight-job-ontology-api-openapi.yml
  format: yaml
  label: Figure Eight Job Ontology API
  slug: figure-eight-job-ontology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-job-ontology-api-openapi.yml
- filename: figure-eight-job-results-api-openapi.yml
  format: yaml
  label: Figure Eight Job Results API
  slug: figure-eight-job-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-job-results-api-openapi.yml
- filename: figure-eight-job-status-api-openapi.yml
  format: yaml
  label: Figure Eight Job Status API
  slug: figure-eight-job-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-job-status-api-openapi.yml
- filename: figure-eight-manage-job-data-api-openapi.yml
  format: yaml
  label: Figure Eight Manage Job Data API
  slug: figure-eight-manage-job-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-manage-job-data-api-openapi.yml
- filename: figure-eight-manage-job-settings-api-openapi.yml
  format: yaml
  label: Figure Eight Manage Job Settings API
  slug: figure-eight-manage-job-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-manage-job-settings-api-openapi.yml
- filename: figure-eight-monitor-contributors-api-openapi.yml
  format: yaml
  label: Figure Eight Monitor Contributors API
  slug: figure-eight-monitor-contributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-monitor-contributors-api-openapi.yml
- filename: figure-eight-workflow-data-upload-download-api-openapi.yml
  format: yaml
  label: Figure Eight Workflow Data Upload/Download API
  slug: figure-eight-workflow-data-upload-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflow-data-upload-download-api-openapi.yml
- filename: figure-eight-workflow-filter-rules-api-openapi.yml
  format: yaml
  label: Figure Eight Workflow Filter Rules API
  slug: figure-eight-workflow-filter-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflow-filter-rules-api-openapi.yml
- filename: figure-eight-workflow-step-routes-api-openapi.yml
  format: yaml
  label: Figure Eight Workflow Step Routes API
  slug: figure-eight-workflow-step-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflow-step-routes-api-openapi.yml
- filename: figure-eight-workflow-steps-api-openapi.yml
  format: yaml
  label: Figure Eight Workflow Steps API
  slug: figure-eight-workflow-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflow-steps-api-openapi.yml
- filename: figure-eight-workflows-api-openapi.yml
  format: yaml
  label: Figure Eight Workflows API
  slug: figure-eight-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swaggerhub.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.appen.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appen.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: app.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.appen.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Figure Eight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figure Eight, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Figure Eight
provider_slug: figure-eight
slug: figure-eight-domain-security
source_filename: figure-eight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.appen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: swaggerhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: appen.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.appen.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/security/figure-eight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Machine Learning
- Data Labeling
- Data Annotation
- Training Data
- Human-in-the-Loop
- Crowdsourcing
- Acquired
---
