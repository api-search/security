---
api_specs:
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Index API
  slug: searchcraft-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Documents / Ingest API
  slug: searchcraft-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Search API
  slug: searchcraft-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Federated Search API
  slug: searchcraft-federated-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
- filename: searchcraft-openapi.yml
  format: yaml
  label: Searchcraft Synonyms & Stopwords API
  slug: searchcraft-synonyms-stopwords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/openapi/searchcraft-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: searchcraft.io
  spf: true
hosts:
- cert_expires: Aug 16 16:42:27 2026 GMT
  host: www.searchcraft.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: docs.searchcraft.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-cluster.searchcraft.io
  https: false
kind: domain-security
layout: security
method: probed
name: Searchcraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Searchcraft, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Searchcraft
provider_slug: searchcraft
slug: searchcraft-domain-security
source_filename: searchcraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.searchcraft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.searchcraft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\n- host: your-cluster.searchcraft.io\n  https: false\ndomains:\n- domain: searchcraft.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchcraft/refs/heads/main/security/searchcraft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Search as a Service
- Full Text Search
- Indexing
- Developer Tools
---
