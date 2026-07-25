---
api_specs:
- filename: spinnaker-applications-api-openapi.yml
  format: yaml
  label: Spinnaker Applications API
  slug: spinnaker-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-applications-api-openapi.yml
- filename: spinnaker-build-services-api-openapi.yml
  format: yaml
  label: Spinnaker Build Services API
  slug: spinnaker-build-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-build-services-api-openapi.yml
- filename: spinnaker-clusters-api-openapi.yml
  format: yaml
  label: Spinnaker Clusters API
  slug: spinnaker-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-clusters-api-openapi.yml
- filename: spinnaker-images-api-openapi.yml
  format: yaml
  label: Spinnaker Images API
  slug: spinnaker-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-images-api-openapi.yml
- filename: spinnaker-load-balancers-api-openapi.yml
  format: yaml
  label: Spinnaker Load Balancers API
  slug: spinnaker-load-balancers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-load-balancers-api-openapi.yml
- filename: spinnaker-pipelines-api-openapi.yml
  format: yaml
  label: Spinnaker Pipelines API
  slug: spinnaker-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-pipelines-api-openapi.yml
- filename: spinnaker-projects-api-openapi.yml
  format: yaml
  label: Spinnaker Projects API
  slug: spinnaker-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-projects-api-openapi.yml
- filename: spinnaker-search-api-openapi.yml
  format: yaml
  label: Spinnaker Search API
  slug: spinnaker-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-search-api-openapi.yml
- filename: spinnaker-tasks-api-openapi.yml
  format: yaml
  label: Spinnaker Tasks API
  slug: spinnaker-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spinnaker.io
  spf: false
hosts:
- cert_expires: Aug 29 03:13:50 2026 GMT
  host: spinnaker.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spinnaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spinnaker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Spinnaker
provider_slug: spinnaker
slug: spinnaker-domain-security
source_filename: spinnaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spinnaker.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 03:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spinnaker.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/security/spinnaker-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Continuous Delivery
- Containers
- DevOps
- Multi-Cloud
- Pipelines
---
