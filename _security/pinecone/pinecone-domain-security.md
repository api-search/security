---
api_specs:
- filename: pinecone-db-control-openapi.yaml
  format: yaml
  label: Pinecone Database Control API
  slug: pinecone-database-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-db-control-openapi.yaml
- filename: pinecone-db-data-openapi.yaml
  format: yaml
  label: Pinecone Database Data API
  slug: pinecone-database-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-db-data-openapi.yaml
- filename: pinecone-inference-openapi.yaml
  format: yaml
  label: Pinecone Inference API
  slug: pinecone-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-inference-openapi.yaml
- filename: pinecone-assistant-control-openapi.yaml
  format: yaml
  label: Pinecone Assistant Control API
  slug: pinecone-assistant-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-assistant-control-openapi.yaml
- filename: pinecone-assistant-data-openapi.yaml
  format: yaml
  label: Pinecone Assistant Data API
  slug: pinecone-assistant-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-assistant-data-openapi.yaml
- filename: pinecone-admin-openapi.yaml
  format: yaml
  label: Pinecone Admin API
  slug: pinecone-admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/openapi/pinecone-admin-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@pinecone.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pinecone.io
  spf: true
hosts:
- cert_expires: Aug 29 08:14:09 2026 GMT
  host: www.pinecone.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 10:05:19 2026 GMT
  host: docs.pinecone.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 18:20:12 2026 GMT
  host: api.pinecone.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinecone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinecone, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Pinecone
provider_slug: pinecone
slug: pinecone-domain-security
source_filename: pinecone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinecone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:14:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.pinecone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:05:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pinecone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:20:12 2026 GMT\n  hsts: null\ndomains:\n- domain: pinecone.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@pinecone.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinecone/refs/heads/main/security/pinecone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Vector Databases
- AI
- Embeddings
- RAG
---
