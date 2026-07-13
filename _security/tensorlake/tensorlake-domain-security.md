---
api_specs:
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Document Parse API
  slug: tensorlake-document-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Structured Extraction API
  slug: tensorlake-structured-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Files API
  slug: tensorlake-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Datasets API
  slug: tensorlake-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Sandboxes API
  slug: tensorlake-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tensorlake.ai
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Sep 16 22:25:50 2026 GMT
  cert_issuer: Let's Encrypt
  host: tensorlake.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  notes: 307 redirect to https://www.tensorlake.ai/ (Vercel).
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: api.tensorlake.ai
  hsts: null
  https: true
  notes: AWS ELB origin. Unauthenticated request returns HTTP 401 (Bearer enforced). No HSTS header observed on the 401 response.
- cert_expires: Sep 25 06:23:25 2026 GMT
  cert_issuer: Let's Encrypt
  host: docs.tensorlake.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  notes: 308 redirect to /sandboxes/introduction (Vercel).
  tls_version: TLSv1.3
- cert_expires: Aug 18 21:56:56 2026 GMT
  cert_issuer: Let's Encrypt
  host: cloud.tensorlake.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  notes: 307 redirect to /login (Vercel).
kind: domain-security
layout: security
method: probed
name: Tensorlake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tensorlake, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tensorlake
provider_slug: tensorlake
slug: tensorlake-domain-security
source_filename: tensorlake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tensorlake.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep 16 22:25:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  notes: 307 redirect to https://www.tensorlake.ai/ (Vercel).\n- host: api.tensorlake.ai\n  https: true\n  cert_issuer: Amazon RSA 2048 M04\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\n  notes: AWS ELB origin. Unauthenticated request returns HTTP 401 (Bearer enforced). No HSTS header observed on the 401 response.\n- host: docs.tensorlake.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep 25 06:23:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  notes: 308 redirect to /sandboxes/introduction (Vercel).\n- host: cloud.tensorlake.ai\n  https: true\n  cert_issuer: Let's Encrypt\n  cert_expires: Aug 18 21:56:56 2026 GMT\n  hsts: true\n  hsts_max_age:\
  \ 63072000\n  notes: 307 redirect to /login (Vercel).\ndomains:\n- domain: tensorlake.ai\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com ~all'\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/security/tensorlake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Extraction
- Data Extraction
- Document Ingestion
- Document Parsing
- OCR
- Data Ingestion
- AI
- Unstructured Data
- Document AI
- RAG
---
