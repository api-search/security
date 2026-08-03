---
api_specs:
- filename: truefoundry-audio-api-openapi.yml
  format: yaml
  label: TrueFoundry Audio API
  slug: truefoundry-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-audio-api-openapi.yml
- filename: truefoundry-batches-api-openapi.yml
  format: yaml
  label: TrueFoundry Batches API
  slug: truefoundry-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-batches-api-openapi.yml
- filename: truefoundry-chat-api-openapi.yml
  format: yaml
  label: TrueFoundry Chat API
  slug: truefoundry-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-chat-api-openapi.yml
- filename: truefoundry-embeddings-api-openapi.yml
  format: yaml
  label: TrueFoundry Embeddings API
  slug: truefoundry-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-embeddings-api-openapi.yml
- filename: truefoundry-files-api-openapi.yml
  format: yaml
  label: TrueFoundry Files API
  slug: truefoundry-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-files-api-openapi.yml
- filename: truefoundry-images-api-openapi.yml
  format: yaml
  label: TrueFoundry Images API
  slug: truefoundry-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-images-api-openapi.yml
- filename: truefoundry-models-api-openapi.yml
  format: yaml
  label: TrueFoundry Models API
  slug: truefoundry-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-models-api-openapi.yml
- filename: truefoundry-moderations-api-openapi.yml
  format: yaml
  label: TrueFoundry Moderations API
  slug: truefoundry-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-moderations-api-openapi.yml
- filename: truefoundry-rerank-api-openapi.yml
  format: yaml
  label: TrueFoundry Rerank API
  slug: truefoundry-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/openapi/truefoundry-rerank-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: truefoundry.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: truefoundry.ai
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.truefoundry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 15:04:18 2026 GMT
  host: gateway.truefoundry.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: app.truefoundry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truefoundry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueFoundry, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TrueFoundry
provider_slug: truefoundry
slug: truefoundry-domain-security
source_filename: truefoundry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truefoundry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.truefoundry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:04:18 2026 GMT\n  hsts: false\n- host: app.truefoundry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: truefoundry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: truefoundry.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truefoundry/refs/heads/main/security/truefoundry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Platform
- Enterprise AI
- Kubernetes
- LLM Gateway
- MLOps
---
