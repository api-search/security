---
api_specs:
- filename: insforge-auth-openapi.yaml
  format: yaml
  label: Insforge Authentication API
  slug: insforge-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-auth-openapi.yaml
- filename: insforge-payments-openapi.yaml
  format: yaml
  label: Insforge Payments API
  slug: insforge-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-payments-openapi.yaml
- filename: insforge-storage-openapi.yaml
  format: yaml
  label: Insforge Storage API
  slug: insforge-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-storage-openapi.yaml
- filename: insforge-deployments-openapi.yaml
  format: yaml
  label: Insforge Deployments API
  slug: insforge-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-deployments-openapi.yaml
- filename: insforge-realtime-openapi.yaml
  format: yaml
  label: Insforge Realtime API
  slug: insforge-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-realtime-openapi.yaml
- filename: insforge-functions-openapi.yaml
  format: yaml
  label: Insforge Functions API
  slug: insforge-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-functions-openapi.yaml
- filename: insforge-ai-openapi.yaml
  format: yaml
  label: Insforge AI API
  slug: insforge-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-ai-openapi.yaml
- filename: insforge-tables-openapi.yaml
  format: yaml
  label: Insforge Tables API
  slug: insforge-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-tables-openapi.yaml
- filename: insforge-records-openapi.yaml
  format: yaml
  label: Insforge Records API
  slug: insforge-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-records-openapi.yaml
- filename: insforge-metadata-openapi.yaml
  format: yaml
  label: Insforge Metadata API
  slug: insforge-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-metadata-openapi.yaml
- filename: insforge-secrets-openapi.yaml
  format: yaml
  label: Insforge Secrets API
  slug: insforge-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-secrets-openapi.yaml
- filename: insforge-email-openapi.yaml
  format: yaml
  label: Insforge Email API
  slug: insforge-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-email-openapi.yaml
- filename: insforge-logs-openapi.yaml
  format: yaml
  label: Insforge Logs API
  slug: insforge-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-logs-openapi.yaml
- filename: insforge-health-openapi.yaml
  format: yaml
  label: Insforge Health API
  slug: insforge-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-health-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: insforge.dev
  spf: true
hosts:
- cert_expires: Sep  7 21:24:55 2026 GMT
  host: insforge.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:28:21 2026 GMT
  host: docs.insforge.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.insforge.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insforge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insforge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Insforge
provider_slug: insforge
slug: insforge-domain-security
source_filename: insforge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insforge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:24:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.insforge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.insforge.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: insforge.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/security/insforge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Backend as a Service
- Agent Native
- Cloud Infrastructure
- Database
- Authentication
- Storage
- Serverless
- Edge Functions
- AI Gateway
- Payments
- Realtime
- Open Source
- Y Combinator
---
