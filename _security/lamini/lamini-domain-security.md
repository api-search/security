---
api_specs:
- filename: lamini-embeddings-api-openapi.yml
  format: yaml
  label: Lamini Embeddings API
  slug: lamini-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-embeddings-api-openapi.yml
- filename: lamini-classifier-api-openapi.yml
  format: yaml
  label: Lamini Classifier API
  slug: lamini-classifier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-classifier-api-openapi.yml
- filename: lamini-completions-api-openapi.yml
  format: yaml
  label: Lamini Completions API
  slug: lamini-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-completions-api-openapi.yml
- filename: lamini-memory-rag-api-openapi.yml
  format: yaml
  label: Lamini memory rag API
  slug: lamini-memory-rag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-memory-rag-api-openapi.yml
- filename: lamini-model-management-api-openapi.yml
  format: yaml
  label: Lamini model management API
  slug: lamini-model-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-model-management-api-openapi.yml
- filename: lamini-train-api-openapi.yml
  format: yaml
  label: Lamini Train API
  slug: lamini-train-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamini/openapi/lamini-train-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lamini.ai
  spf: true
hosts:
- host: www.lamini.ai
  https: false
- cert_expires: Sep 19 03:26:50 2026 GMT
  host: docs.lamini.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 03:26:50 2026 GMT
  host: api.lamini.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Lamini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lamini, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lamini
provider_slug: lamini
slug: lamini-domain-security
source_filename: lamini-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lamini.ai\n  https: false\n- host: docs.lamini.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:26:50 2026 GMT\n  hsts: false\n- host: api.lamini.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:26:50 2026 GMT\n  hsts: null\ndomains:\n- domain: lamini.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lamini/security/lamini-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- LLM
- Fine-Tuning
- Memory Tuning
- Inference
---
