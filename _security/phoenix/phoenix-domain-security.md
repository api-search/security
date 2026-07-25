---
api_specs:
- filename: phoenix-annotation-configs-api-openapi.yml
  format: yaml
  label: Arize Phoenix annotation_configs API
  slug: phoenix-annotation-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-annotation-configs-api-openapi.yml
- filename: phoenix-annotations-api-openapi.yml
  format: yaml
  label: Arize Phoenix annotations API
  slug: phoenix-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-annotations-api-openapi.yml
- filename: phoenix-arize-phoenix-version-api-openapi.yml
  format: yaml
  label: Arize Phoenix Arize Phoenix Version API
  slug: phoenix-arize-phoenix-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-arize-phoenix-version-api-openapi.yml
- filename: phoenix-auth-api-openapi.yml
  format: yaml
  label: Arize Phoenix Auth API
  slug: phoenix-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-auth-api-openapi.yml
- filename: phoenix-chat-api-openapi.yml
  format: yaml
  label: Arize Phoenix chat API
  slug: phoenix-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-chat-api-openapi.yml
- filename: phoenix-datasets-api-openapi.yml
  format: yaml
  label: Arize Phoenix datasets API
  slug: phoenix-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-datasets-api-openapi.yml
- filename: phoenix-experiments-api-openapi.yml
  format: yaml
  label: Arize Phoenix experiments API
  slug: phoenix-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-experiments-api-openapi.yml
- filename: phoenix-healthz-api-openapi.yml
  format: yaml
  label: Arize Phoenix Healthz API
  slug: phoenix-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-healthz-api-openapi.yml
- filename: phoenix-oauth2-api-openapi.yml
  format: yaml
  label: Arize Phoenix Oauth2 API
  slug: phoenix-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-oauth2-api-openapi.yml
- filename: phoenix-projects-api-openapi.yml
  format: yaml
  label: Arize Phoenix projects API
  slug: phoenix-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-projects-api-openapi.yml
- filename: phoenix-prompts-api-openapi.yml
  format: yaml
  label: Arize Phoenix prompts API
  slug: phoenix-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-prompts-api-openapi.yml
- filename: phoenix-readyz-api-openapi.yml
  format: yaml
  label: Arize Phoenix Readyz API
  slug: phoenix-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-readyz-api-openapi.yml
- filename: phoenix-secrets-api-openapi.yml
  format: yaml
  label: Arize Phoenix secrets API
  slug: phoenix-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-secrets-api-openapi.yml
- filename: phoenix-sessions-api-openapi.yml
  format: yaml
  label: Arize Phoenix sessions API
  slug: phoenix-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-sessions-api-openapi.yml
- filename: phoenix-spans-api-openapi.yml
  format: yaml
  label: Arize Phoenix spans API
  slug: phoenix-spans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-spans-api-openapi.yml
- filename: phoenix-traces-api-openapi.yml
  format: yaml
  label: Arize Phoenix traces API
  slug: phoenix-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-traces-api-openapi.yml
- filename: phoenix-users-api-openapi.yml
  format: yaml
  label: Arize Phoenix users API
  slug: phoenix-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/openapi/phoenix-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arize.com
  spf: true
hosts:
- cert_expires: Aug 15 02:12:54 2026 GMT
  host: arize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 12:54:56 2026 GMT
  host: app.phoenix.arize.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phoenix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arize Phoenix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arize Phoenix
provider_slug: phoenix
slug: phoenix-domain-security
source_filename: phoenix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 02:12:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.phoenix.arize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: arize.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phoenix/refs/heads/main/security/phoenix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LLM Observability
- AI Evaluation
- OpenTelemetry
- Tracing
- LLMOps
- AI Monitoring
- Open Source
- Prompt Engineering
- Datasets
- Experiments
---
