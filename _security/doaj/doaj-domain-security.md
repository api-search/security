---
api_specs:
- filename: doaj-bulk-api-api-openapi.yml
  format: yaml
  label: DOAJ Bulk API
  slug: doaj-bulk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doaj/refs/heads/main/openapi/doaj-bulk-api-api-openapi.yml
- filename: doaj-crud-applications-api-openapi.yml
  format: yaml
  label: DOAJ CRUD Applications API
  slug: doaj-crud-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doaj/refs/heads/main/openapi/doaj-crud-applications-api-openapi.yml
- filename: doaj-crud-articles-api-openapi.yml
  format: yaml
  label: DOAJ CRUD Articles API
  slug: doaj-crud-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doaj/refs/heads/main/openapi/doaj-crud-articles-api-openapi.yml
- filename: doaj-crud-journals-api-openapi.yml
  format: yaml
  label: DOAJ CRUD Journals API
  slug: doaj-crud-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doaj/refs/heads/main/openapi/doaj-crud-journals-api-openapi.yml
- filename: doaj-search-api-openapi.yml
  format: yaml
  label: DOAJ Search API
  slug: doaj-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doaj/refs/heads/main/openapi/doaj-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: doaj.org
  spf: true
hosts:
- cert_expires: Jan 11 05:21:31 2027 GMT
  host: doaj.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Doaj Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DOAJ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DOAJ
provider_slug: doaj
slug: doaj-domain-security
source_filename: doaj-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doaj.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 05:21:31 2027 GMT\n  hsts: null\ndomains:\n- domain: doaj.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doaj/refs/heads/main/security/doaj-domain-security.yml
summary_line: TLSv1.3
tags:
- OpenAccess
- Journals
- ScholarlyPublishing
- Metadata
---
