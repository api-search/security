---
api_specs:
- filename: openapi.json
  format: json
  label: Hugging Face Inference API
  slug: hugging-face-inference-api
  spec_type: OpenAPI
  url: https://huggingface.co/api-inference/openapi.json
- filename: openapi.json
  format: json
  label: Hugging Face Hub API
  slug: hugging-face-hub-api
  spec_type: OpenAPI
  url: https://huggingface.co/.well-known/openapi.json
- filename: hugging-face-inference-endpoints-api.yml
  format: yaml
  label: Hugging Face Inference Endpoints API
  slug: hugging-face-inference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/openapi/hugging-face-inference-endpoints-api.yml
- filename: hugging-face-inference-providers-api.yml
  format: yaml
  label: Hugging Face Inference Providers API
  slug: hugging-face-inference-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/openapi/hugging-face-inference-providers-api.yml
- filename: openapi.json
  format: json
  label: Hugging Face Dataset Viewer API
  slug: hugging-face-dataset-viewer-api
  spec_type: OpenAPI
  url: https://datasets-server.huggingface.co/openapi.json
- filename: hugging-face-text-generation-inference-api.yml
  format: yaml
  label: Hugging Face Text Generation Inference API
  slug: hugging-face-text-generation-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/openapi/hugging-face-text-generation-inference-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: huggingface.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: huggingface.cloud
  spf: false
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: huggingface.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api-inference.huggingface.co
  https: false
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.endpoints.huggingface.cloud
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hugging Face Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hugging Face, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hugging Face
provider_slug: hugging-face
slug: hugging-face-domain-security
source_filename: hugging-face-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huggingface.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\n- host: api-inference.huggingface.co\n  https: false\n- host: api.endpoints.huggingface.cloud\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: huggingface.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: huggingface.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/security/hugging-face-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags: []
---
