---
api_specs:
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Knowledge Boxes API
  slug: knowledge-boxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Resources & Ingestion API
  slug: resources-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Search & Find API
  slug: search-find-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Ask & Chat (RAG) API
  slug: ask-chat-rag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
- filename: nuclia-openapi.yml
  format: yaml
  label: Nuclia Predict (NUA) API
  slug: predict-nua-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/openapi/nuclia-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nuclia.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nuclia.dev
  spf: false
hosts:
- cert_expires: Sep 21 12:51:31 2026 GMT
  host: nuclia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: docs.nuclia.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuclia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuclia, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nuclia
provider_slug: nuclia
slug: nuclia-domain-security
source_filename: nuclia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuclia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:51:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nuclia.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nuclia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nuclia.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuclia/refs/heads/main/security/nuclia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- RAG
- Search
- Knowledge Base
- Unstructured Data
---
