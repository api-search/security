---
api_specs:
- filename: lance-namespace-openapi.yaml
  format: yaml
  label: LanceDB OSS
  slug: oss
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/main/openapi/lance-namespace-openapi.yaml
- filename: lance-namespace-openapi.yaml
  format: yaml
  label: LanceDB Cloud
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lancedb/main/openapi/lance-namespace-openapi.yaml
- filename: spec.yaml
  format: yaml
  label: Lance Namespace Specification
  slug: lance-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/lance-format/lance-namespace/main/docs/src/spec.yaml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lancedb.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lancedb.cloud
  spf: true
hosts:
- cert_expires: Aug 30 01:11:11 2026 GMT
  host: lancedb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 13:53:03 2026 GMT
  host: docs.lancedb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: your-tenant.lancedb.cloud
  https: false
kind: domain-security
layout: security
method: probed
name: Lancedb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LanceDB, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LanceDB
provider_slug: lancedb
slug: lancedb-domain-security
source_filename: lancedb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lancedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:11:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lancedb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 13:53:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-tenant.lancedb.cloud\n  https: false\ndomains:\n- domain: lancedb.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lancedb.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lancedb/refs/heads/main/security/lancedb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vector Database
- Multimodal
- Lance Format
- Lakehouse
- RAG
- Agent Memory
- Open Source
- Embeddings
- Full-Text Search
- Hybrid Search
- Columnar Storage
- Arrow
- AI Infrastructure
---
