---
api_specs:
- filename: statorigin-indicators-api-openapi.yml
  format: yaml
  label: StatOrigin Indicators API
  slug: statorigin-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-indicators-api-openapi.yml
- filename: statorigin-industries-api-openapi.yml
  format: yaml
  label: StatOrigin Industries API
  slug: statorigin-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-industries-api-openapi.yml
- filename: statorigin-regions-api-openapi.yml
  format: yaml
  label: StatOrigin Regions API
  slug: statorigin-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-regions-api-openapi.yml
- filename: statorigin-search-api-openapi.yml
  format: yaml
  label: StatOrigin Search API
  slug: statorigin-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-search-api-openapi.yml
- filename: statorigin-sources-api-openapi.yml
  format: yaml
  label: StatOrigin Sources API
  slug: statorigin-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-sources-api-openapi.yml
- filename: statorigin-statistics-api-openapi.yml
  format: yaml
  label: StatOrigin Statistics API
  slug: statorigin-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/openapi/statorigin-statistics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: statorigin.org
  spf: true
hosts:
- cert_expires: Dec 14 08:28:23 2026 GMT
  host: statorigin.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Statorigin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StatOrigin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StatOrigin
provider_slug: statorigin
slug: statorigin-domain-security
source_filename: statorigin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: statorigin.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 08:28:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: statorigin.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statorigin/refs/heads/main/security/statorigin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Statistics
- OpenAPI
- Free
---
