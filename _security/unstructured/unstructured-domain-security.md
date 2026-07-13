---
api_specs:
- filename: unstructured-platform-api-openapi.yml
  format: yaml
  label: Unstructured Platform API
  slug: unstructured-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-platform-api-openapi.yml
- filename: unstructured-partition-endpoint-openapi.yml
  format: yaml
  label: Unstructured Partition Endpoint
  slug: unstructured-partition-endpoint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/openapi/unstructured-partition-endpoint-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:infosec@unstructured.io"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unstructured.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unstructuredapp.io
  spf: true
hosts:
- cert_expires: Sep  8 09:16:54 2026 GMT
  host: unstructured.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 17:22:19 2026 GMT
  host: docs.unstructured.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 10:53:54 2026 GMT
  host: platform.unstructuredapp.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unstructured Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unstructured, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unstructured
provider_slug: unstructured
slug: unstructured-domain-security
source_filename: unstructured-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unstructured.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:16:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.unstructured.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 17:22:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.unstructuredapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:53:54 2026 GMT\n  hsts: null\ndomains:\n- domain: unstructured.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:infosec@unstructured.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: unstructuredapp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unstructured/refs/heads/main/security/unstructured-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- document-processing
- ETL
- RAG
- LLM
- PDF
- OCR
- data-ingestion
- chunking
- embeddings
- AI
---
