---
api_specs:
- filename: unfao-catalog-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Catalog API
  slug: unfao-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-catalog-api-openapi.yml
- filename: unfao-data-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Data API
  slug: unfao-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-data-api-openapi.yml
- filename: unfao-dimensions-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Dimensions API
  slug: unfao-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-dimensions-api-openapi.yml
- filename: unfao-domains-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Domains API
  slug: unfao-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-domains-api-openapi.yml
- filename: unfao-downloads-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Downloads API
  slug: unfao-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-downloads-api-openapi.yml
- filename: unfao-metadata-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Metadata API
  slug: unfao-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-metadata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fao.org
  spf: true
hosts:
- cert_expires: Sep 10 04:16:19 2026 GMT
  host: www.fao.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 02:38:56 2026 GMT
  host: fenixservices.fao.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: bulks-faostat.fao.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unfao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FAO FAOSTAT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FAO FAOSTAT
provider_slug: unfao
slug: unfao-domain-security
source_filename: unfao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:16:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fenixservices.fao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:38:56 2026 GMT\n  hsts: null\n- host: bulks-faostat.fao.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: fao.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/security/unfao-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Food Security
- Statistics
- Trade
- Land Use
- Environment
- UN
- Open Data
---
