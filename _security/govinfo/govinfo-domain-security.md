---
api_specs:
- filename: govinfo-collections-api-openapi.yml
  format: yaml
  label: GovInfo Collections API
  slug: govinfo-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-collections-api-openapi.yml
- filename: govinfo-packages-api-openapi.yml
  format: yaml
  label: GovInfo Packages API
  slug: govinfo-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-packages-api-openapi.yml
- filename: govinfo-published-api-openapi.yml
  format: yaml
  label: GovInfo Published API
  slug: govinfo-published-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-published-api-openapi.yml
- filename: govinfo-related-api-openapi.yml
  format: yaml
  label: GovInfo Related API
  slug: govinfo-related-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-related-api-openapi.yml
- filename: govinfo-search-api-openapi.yml
  format: yaml
  label: GovInfo Search API
  slug: govinfo-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: govinfo.gov
  spf: false
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.govinfo.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 15:21:32 2026 GMT
  host: api.govinfo.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Govinfo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GovInfo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: GovInfo
provider_slug: govinfo
slug: govinfo-domain-security
source_filename: govinfo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.govinfo.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.govinfo.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govinfo.gov\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/security/govinfo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Federal Government
- Government Publishing
- Documents
- Open Data
---
