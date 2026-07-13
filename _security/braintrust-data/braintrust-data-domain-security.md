---
api_specs:
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Projects API
  slug: braintrust-data-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Experiments API
  slug: braintrust-data-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Datasets API
  slug: braintrust-data-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Logs and Spans API
  slug: braintrust-data-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Prompts API
  slug: braintrust-data-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Functions and Scorers API
  slug: braintrust-data-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Project Configuration API
  slug: braintrust-data-project-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Organization and ACL API
  slug: braintrust-data-acl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust Credentials and Secrets API
  slug: braintrust-data-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
- filename: braintrust-data-openapi.yml
  format: yaml
  label: Braintrust AI Proxy API
  slug: braintrust-data-ai-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: braintrust.dev
  spf: true
hosts:
- cert_expires: Sep 22 20:45:31 2026 GMT
  host: www.braintrust.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.braintrust.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api-eu.braintrust.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Braintrust Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braintrust, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Braintrust
provider_slug: braintrust-data
slug: braintrust-data-domain-security
source_filename: braintrust-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.braintrust.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:45:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.braintrust.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\n- host: api-eu.braintrust.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: braintrust.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/security/braintrust-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Evaluation
- Observability
- LLMOps
---
