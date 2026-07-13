---
api_specs:
- filename: typesense-search-api-openapi.yml
  format: yaml
  label: Typesense Search API
  slug: typesense-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-search-api-openapi.yml
- filename: typesense-vector-search-api-openapi.yml
  format: yaml
  label: Typesense Vector Search API
  slug: typesense-vector-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-vector-search-api-openapi.yml
- filename: typesense-conversational-search-api-openapi.yml
  format: yaml
  label: Typesense Conversational Search API
  slug: typesense-conversational-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-conversational-search-api-openapi.yml
- filename: typesense-analytics-api-openapi.yml
  format: yaml
  label: Typesense Analytics API
  slug: typesense-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-analytics-api-openapi.yml
- filename: typesense-cloud-management-api-openapi.yml
  format: yaml
  label: Typesense Cloud Management API
  slug: typesense-cloud-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/openapi/typesense-cloud-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: typesense.org
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: typesense.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: cloud.typesense.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Typesense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Typesense, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Typesense
provider_slug: typesense
slug: typesense-domain-security
source_filename: typesense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: typesense.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: cloud.typesense.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: typesense.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typesense/refs/heads/main/security/typesense-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Full-Text Search
- Open Source
- Search Engine
- Typo Tolerance
- Vector Search
---
