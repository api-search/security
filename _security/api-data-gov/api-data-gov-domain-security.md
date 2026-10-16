---
api_specs:
- filename: api-data-gov-dataset-api-openapi.yml
  format: yaml
  label: api.data.gov Dataset API
  slug: api-data-gov-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-dataset-api-openapi.yml
- filename: api-data-gov-harvest-jobs-api-openapi.yml
  format: yaml
  label: api.data.gov Harvest Jobs API
  slug: api-data-gov-harvest-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-harvest-jobs-api-openapi.yml
- filename: api-data-gov-harvest-records-api-openapi.yml
  format: yaml
  label: api.data.gov Harvest Records API
  slug: api-data-gov-harvest-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-harvest-records-api-openapi.yml
- filename: api-data-gov-harvest-sources-api-openapi.yml
  format: yaml
  label: api.data.gov Harvest Sources API
  slug: api-data-gov-harvest-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-harvest-sources-api-openapi.yml
- filename: api-data-gov-keywords-api-openapi.yml
  format: yaml
  label: api.data.gov Keywords API
  slug: api-data-gov-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-keywords-api-openapi.yml
- filename: api-data-gov-location-api-openapi.yml
  format: yaml
  label: api.data.gov Location API
  slug: api-data-gov-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-location-api-openapi.yml
- filename: api-data-gov-locations-api-openapi.yml
  format: yaml
  label: api.data.gov Locations API
  slug: api-data-gov-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-locations-api-openapi.yml
- filename: api-data-gov-organizations-api-openapi.yml
  format: yaml
  label: api.data.gov Organizations API
  slug: api-data-gov-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-organizations-api-openapi.yml
- filename: api-data-gov-publishers-api-openapi.yml
  format: yaml
  label: api.data.gov Publishers API
  slug: api-data-gov-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-publishers-api-openapi.yml
- filename: api-data-gov-search-api-openapi.yml
  format: yaml
  label: api.data.gov Search API
  slug: api-data-gov-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-search-api-openapi.yml
- filename: api-data-gov-stats-api-openapi.yml
  format: yaml
  label: api.data.gov Stats API
  slug: api-data-gov-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-stats-api-openapi.yml
- filename: api-data-gov-validate-api-openapi.yml
  format: yaml
  label: api.data.gov Validate API
  slug: api-data-gov-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-validate-api-openapi.yml
- filename: api-data-gov-open-search-api-openapi.yml
  format: yaml
  label: api.data.gov Open Search API
  slug: api-data-gov-open-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-open-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: data.gov
  spf: true
hosts:
- cert_expires: Nov 15 14:21:13 2026 GMT
  host: api.data.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Api Data Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for api.data.gov, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: api.data.gov
provider_slug: api-data-gov
slug: api-data-gov-domain-security
source_filename: api-data-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 14:21:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/security/api-data-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Data
- API
- Open-Data
---
