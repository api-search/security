---
api_specs:
- filename: restate-cluster-health-api-openapi.yml
  format: yaml
  label: Restate cluster_health API
  slug: restate-cluster-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-cluster-health-api-openapi.yml
- filename: restate-deployment-api-openapi.yml
  format: yaml
  label: Restate deployment API
  slug: restate-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-deployment-api-openapi.yml
- filename: restate-health-api-openapi.yml
  format: yaml
  label: Restate health API
  slug: restate-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-health-api-openapi.yml
- filename: restate-invocation-api-openapi.yml
  format: yaml
  label: Restate invocation API
  slug: restate-invocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-invocation-api-openapi.yml
- filename: restate-openapi-api-openapi.yml
  format: yaml
  label: Restate openapi API
  slug: restate-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-openapi-api-openapi.yml
- filename: restate-service-api-openapi.yml
  format: yaml
  label: Restate service API
  slug: restate-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-service-api-openapi.yml
- filename: restate-service-handler-api-openapi.yml
  format: yaml
  label: Restate service_handler API
  slug: restate-service-handler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-service-handler-api-openapi.yml
- filename: restate-subscription-api-openapi.yml
  format: yaml
  label: Restate subscription API
  slug: restate-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-subscription-api-openapi.yml
- filename: restate-version-api-openapi.yml
  format: yaml
  label: Restate version API
  slug: restate-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/openapi/restate-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: restate.dev
  spf: true
hosts:
- cert_expires: Aug 31 21:22:25 2026 GMT
  host: restate.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Restate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Restate
provider_slug: restate
slug: restate-domain-security
source_filename: restate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restate.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:22:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: restate.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restate/refs/heads/main/security/restate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Durable Execution
- Workflows
- Microservices
- Orchestration
- Distributed Systems
---
