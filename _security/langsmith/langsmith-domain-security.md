---
api_specs:
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Tracing API
  slug: langsmith-tracing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Datasets API
  slug: langsmith-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Evaluations API
  slug: langsmith-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Prompt Hub API
  slug: langsmith-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Feedback API
  slug: langsmith-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Annotation Queues API
  slug: langsmith-annotation-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
- filename: langsmith-openapi.json
  format: json
  label: LangSmith Fleet (Agent Deployment) API
  slug: langsmith-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/openapi/langsmith-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: langchain.com
  spf: true
hosts:
- cert_expires: Sep 23 23:21:48 2026 GMT
  host: smith.langchain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 16:49:13 2026 GMT
  host: docs.langchain.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:21:48 2026 GMT
  host: api.smith.langchain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Langsmith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LangSmith, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LangSmith
provider_slug: langsmith
slug: langsmith-domain-security
source_filename: langsmith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smith.langchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:21:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.langchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:49:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.smith.langchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:21:48 2026 GMT\n  hsts: null\ndomains:\n- domain: langchain.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langsmith/refs/heads/main/security/langsmith-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- LLM
- Observability
- Evaluations
- LangChain
---
