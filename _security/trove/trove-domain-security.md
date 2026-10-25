---
api_specs:
- filename: trove-contributor-api-openapi.yml
  format: yaml
  label: Trove Contributor API
  slug: trove-contributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-contributor-api-openapi.yml
- filename: trove-list-api-openapi.yml
  format: yaml
  label: Trove List API
  slug: trove-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-list-api-openapi.yml
- filename: trove-newspaper-api-openapi.yml
  format: yaml
  label: Trove Newspaper API
  slug: trove-newspaper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-newspaper-api-openapi.yml
- filename: trove-people-api-openapi.yml
  format: yaml
  label: Trove People API
  slug: trove-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-people-api-openapi.yml
- filename: trove-search-api-openapi.yml
  format: yaml
  label: Trove Search API
  slug: trove-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-search-api-openapi.yml
- filename: trove-work-api-openapi.yml
  format: yaml
  label: Trove Work API
  slug: trove-work-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/openapi/trove-work-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nla.gov.au
  spf: true
hosts:
- cert_expires: Jan 18 03:49:38 2027 GMT
  host: trove.nla.gov.au
  hsts: true
  hsts_max_age: 15811200
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trove
provider_slug: trove
slug: trove-domain-security
source_filename: trove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trove.nla.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 03:49:38 2027 GMT\n  hsts: true\n  hsts_max_age: 15811200\ndomains:\n- domain: nla.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/security/trove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- News
- Public APIs
- Libraries
- Cultural Heritage
- Digitised Newspapers
- Archives
- Open Data
- Australia
- Search
---
