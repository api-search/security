---
api_specs:
- filename: dapr-actors-api-openapi.yml
  format: yaml
  label: Dapr Actors API
  slug: dapr-actors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-actors-api-openapi.yml
- filename: dapr-bindings-api-openapi.yml
  format: yaml
  label: Dapr Bindings API
  slug: dapr-bindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-bindings-api-openapi.yml
- filename: dapr-configuration-api-openapi.yml
  format: yaml
  label: Dapr Configuration API
  slug: dapr-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-configuration-api-openapi.yml
- filename: dapr-cryptography-api-openapi.yml
  format: yaml
  label: Dapr Cryptography API
  slug: dapr-cryptography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-cryptography-api-openapi.yml
- filename: dapr-distributedlock-api-openapi.yml
  format: yaml
  label: Dapr DistributedLock API
  slug: dapr-distributedlock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-distributedlock-api-openapi.yml
- filename: dapr-health-api-openapi.yml
  format: yaml
  label: Dapr Health API
  slug: dapr-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-health-api-openapi.yml
- filename: dapr-jobs-api-openapi.yml
  format: yaml
  label: Dapr Jobs API
  slug: dapr-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-jobs-api-openapi.yml
- filename: dapr-metadata-api-openapi.yml
  format: yaml
  label: Dapr Metadata API
  slug: dapr-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-metadata-api-openapi.yml
- filename: dapr-pubsub-api-openapi.yml
  format: yaml
  label: Dapr PubSub API
  slug: dapr-pubsub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-pubsub-api-openapi.yml
- filename: dapr-secrets-api-openapi.yml
  format: yaml
  label: Dapr Secrets API
  slug: dapr-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-secrets-api-openapi.yml
- filename: dapr-serviceinvocation-api-openapi.yml
  format: yaml
  label: Dapr ServiceInvocation API
  slug: dapr-serviceinvocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-serviceinvocation-api-openapi.yml
- filename: dapr-state-api-openapi.yml
  format: yaml
  label: Dapr State API
  slug: dapr-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-state-api-openapi.yml
- filename: dapr-workflow-api-openapi.yml
  format: yaml
  label: Dapr Workflow API
  slug: dapr-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/openapi/dapr-workflow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dapr.io
  spf: true
hosts:
- cert_expires: Aug 23 06:23:54 2026 GMT
  host: dapr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: docs.dapr.io
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dapr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dapr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dapr
provider_slug: dapr
slug: dapr-domain-security
source_filename: dapr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dapr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:23:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dapr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: dapr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/security/dapr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Distributed Systems
- Microservices
- Platform
- Pub-Sub
- State Management
- Workflows
---
