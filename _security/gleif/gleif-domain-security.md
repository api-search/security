---
api_specs:
- filename: gleif-corporate-relationships-api-openapi.yml
  format: yaml
  label: GLEIF Corporate Relationships API
  slug: gleif-corporate-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-corporate-relationships-api-openapi.yml
- filename: gleif-lei-issuers-api-openapi.yml
  format: yaml
  label: GLEIF LEI Issuers API
  slug: gleif-lei-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-lei-issuers-api-openapi.yml
- filename: gleif-lei-records-api-openapi.yml
  format: yaml
  label: GLEIF LEI Records API
  slug: gleif-lei-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-lei-records-api-openapi.yml
- filename: gleif-reference-data-api-openapi.yml
  format: yaml
  label: GLEIF Reference Data API
  slug: gleif-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-reference-data-api-openapi.yml
- filename: gleif-search-api-openapi.yml
  format: yaml
  label: GLEIF Search API
  slug: gleif-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: false
  dnssec: true
  domain: gleif.org
  spf: true
hosts:
- cert_expires: Nov 30 16:02:17 2026 GMT
  host: www.gleif.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 23 14:52:50 2027 GMT
  host: api.gleif.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gleif Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GLEIF, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: GLEIF
provider_slug: gleif
slug: gleif-domain-security
source_filename: gleif-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gleif.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 16:02:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gleif.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 23 14:52:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gleif.org\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/security/gleif-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Legal Entity Identifier
- LEI
- vLEI
- Financial Data
- Corporate Identity
- Entity Verification
- Reference Data
- Open Data
---
