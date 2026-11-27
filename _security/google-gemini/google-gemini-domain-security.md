---
api_specs:
- filename: google-gemini-auth-tokens-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Auth Tokens API
  slug: google-gemini-auth-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-auth-tokens-api-openapi.yml
- filename: google-gemini-batches-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Batches API
  slug: google-gemini-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-batches-api-openapi.yml
- filename: google-gemini-corpora-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Corpora API
  slug: google-gemini-corpora-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-corpora-api-openapi.yml
- filename: google-gemini-dynamic-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Dynamic API
  slug: google-gemini-dynamic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-dynamic-api-openapi.yml
- filename: google-gemini-environments-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Environments API
  slug: google-gemini-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-environments-api-openapi.yml
- filename: google-gemini-files-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Files API
  slug: google-gemini-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-files-api-openapi.yml
- filename: google-gemini-media-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Media API
  slug: google-gemini-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-media-api-openapi.yml
- filename: google-gemini-models-api-openapi.yml
  format: yaml
  label: Google Gemini Gemini Models API
  slug: google-gemini-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-models-api-openapi.yml
- filename: google-gemini-cachedcontents-api-openapi.yml
  format: yaml
  label: Google Gemini Cached Contents API
  slug: google-gemini-cachedcontents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-cachedcontents-api-openapi.yml
- filename: google-gemini-filesearchstores-api-openapi.yml
  format: yaml
  label: Google Gemini File Search Stores API
  slug: google-gemini-filesearchstores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-filesearchstores-api-openapi.yml
- filename: google-gemini-generatedfiles-api-openapi.yml
  format: yaml
  label: Google Gemini Generated Files API
  slug: google-gemini-generatedfiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-generatedfiles-api-openapi.yml
- filename: google-gemini-tunedmodels-api-openapi.yml
  format: yaml
  label: Google Gemini Tuned Models API
  slug: google-gemini-tunedmodels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-gemini/openapi/google-gemini-tunedmodels-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: google.dev
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Dec 30 19:07:42 2026 GMT
  host: google.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:42 2026 GMT
  host: ai.google.dev
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: generativelanguage.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Gemini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Gemini, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Google Gemini
provider_slug: google-gemini
slug: google-gemini-domain-security
source_filename: google-gemini-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: google.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ai.google.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:42 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: generativelanguage.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.dev\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-gemini/security/google-gemini-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Artificial Intelligence
- Code Generation
- Embeddings
- Generative AI
- Image Generation
- LLM
- Machine Learning
- Multi-Modal
- Real-Time
- Foundation Models
- Agents
- Audio Understanding
- Batch Processing
- Deep Research
- Document Understanding
- Function Calling
- Structured Output
- Text-to-Speech
- Video Generation
- Video Understanding
---
