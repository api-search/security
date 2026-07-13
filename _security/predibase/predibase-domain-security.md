---
api_specs:
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Inference (OpenAI-Compatible) API
  slug: predibase-inference-openai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Prompt / Generate API
  slug: predibase-prompt-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Fine-Tuning API
  slug: predibase-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Adapters API
  slug: predibase-adapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Deployments API
  slug: predibase-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Datasets API
  slug: predibase-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Models API
  slug: predibase-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
- filename: predibase-openapi.yml
  format: yaml
  label: Predibase Batch Inference API
  slug: predibase-batch-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/openapi/predibase-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: predibase.com
  spf: false
hosts:
- cert_expires: Sep 22 15:45:16 2026 GMT
  host: predibase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 15:45:16 2026 GMT
  host: docs.predibase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.app.predibase.com
  https: false
kind: domain-security
layout: security
method: probed
name: Predibase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Predibase, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Predibase
provider_slug: predibase
slug: predibase-domain-security
source_filename: predibase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: predibase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:45:16 2026 GMT\n  hsts: null\n- host: docs.predibase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:45:16 2026 GMT\n  hsts: null\n- host: api.app.predibase.com\n  https: false\ndomains:\n- domain: predibase.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predibase/refs/heads/main/security/predibase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- LLM
- Fine-Tuning
- Inference
- LoRA
---
