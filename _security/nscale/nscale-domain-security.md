---
api_specs:
- filename: nscale-chat-api-openapi.yml
  format: yaml
  label: Nscale Chat API
  slug: nscale-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-chat-api-openapi.yml
- filename: nscale-completions-api-openapi.yml
  format: yaml
  label: Nscale Completions API
  slug: nscale-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-completions-api-openapi.yml
- filename: nscale-embeddings-api-openapi.yml
  format: yaml
  label: Nscale Embeddings API
  slug: nscale-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-embeddings-api-openapi.yml
- filename: nscale-images-api-openapi.yml
  format: yaml
  label: Nscale Images API
  slug: nscale-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-images-api-openapi.yml
- filename: nscale-models-api-openapi.yml
  format: yaml
  label: Nscale Models API
  slug: nscale-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-models-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nscale.com
  spf: true
hosts:
- cert_expires: Sep 28 19:01:28 2026 GMT
  host: www.nscale.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 14:35:27 2026 GMT
  host: docs.nscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 21:34:56 2026 GMT
  host: inference.api.nscale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nscale, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nscale
provider_slug: nscale
slug: nscale-domain-security
source_filename: nscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:01:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:35:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: inference.api.nscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 21:34:56 2026 GMT\n  hsts: null\ndomains:\n- domain: nscale.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/security/nscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- GPU
- Inference
- Serverless
- Cloud Compute
---
