---
api_specs:
- filename: zincsearch-document-api-openapi.yml
  format: yaml
  label: ZincSearch Document API
  slug: zincsearch-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-document-api-openapi.yml
- filename: zincsearch-healthz-api-openapi.yml
  format: yaml
  label: ZincSearch Healthz API
  slug: zincsearch-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-healthz-api-openapi.yml
- filename: zincsearch-index-api-openapi.yml
  format: yaml
  label: ZincSearch Index API
  slug: zincsearch-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-index-api-openapi.yml
- filename: zincsearch-permission-api-openapi.yml
  format: yaml
  label: ZincSearch Permission API
  slug: zincsearch-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-permission-api-openapi.yml
- filename: zincsearch-role-api-openapi.yml
  format: yaml
  label: ZincSearch Role API
  slug: zincsearch-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-role-api-openapi.yml
- filename: zincsearch-search-api-openapi.yml
  format: yaml
  label: ZincSearch Search API
  slug: zincsearch-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-search-api-openapi.yml
- filename: zincsearch-user-api-openapi.yml
  format: yaml
  label: ZincSearch User API
  slug: zincsearch-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-user-api-openapi.yml
- filename: zincsearch-version-api-openapi.yml
  format: yaml
  label: ZincSearch Version API
  slug: zincsearch-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/openapi/zincsearch-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zincsearch.com
  spf: false
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: zincsearch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zincsearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZincSearch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ZincSearch
provider_slug: zincsearch
slug: zincsearch-domain-security
source_filename: zincsearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zincsearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zincsearch.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zincsearch/refs/heads/main/security/zincsearch-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Search
- Full-Text Search
- Open Source
- Self-Hosted
- Elasticsearch Compatible
---
