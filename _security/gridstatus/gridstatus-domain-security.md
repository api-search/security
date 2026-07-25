---
api_specs:
- filename: gridstatus-api-info-api-openapi.yml
  format: yaml
  label: Grid Status API Info API
  slug: gridstatus-api-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-api-info-api-openapi.yml
- filename: gridstatus-api-usage-api-openapi.yml
  format: yaml
  label: Grid Status API Usage API
  slug: gridstatus-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-api-usage-api-openapi.yml
- filename: gridstatus-block-pricing-data-api-openapi.yml
  format: yaml
  label: Grid Status Block Pricing Data API
  slug: gridstatus-block-pricing-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-block-pricing-data-api-openapi.yml
- filename: gridstatus-constraints-api-openapi.yml
  format: yaml
  label: Grid Status Constraints API
  slug: gridstatus-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-constraints-api-openapi.yml
- filename: gridstatus-csv-exports-api-openapi.yml
  format: yaml
  label: Grid Status CSV Exports API
  slug: gridstatus-csv-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-csv-exports-api-openapi.yml
- filename: gridstatus-dataset-audit-api-openapi.yml
  format: yaml
  label: Grid Status Dataset Audit API
  slug: gridstatus-dataset-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-dataset-audit-api-openapi.yml
- filename: gridstatus-dataset-metadata-api-openapi.yml
  format: yaml
  label: Grid Status Dataset Metadata API
  slug: gridstatus-dataset-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-dataset-metadata-api-openapi.yml
- filename: gridstatus-dataset-updates-api-openapi.yml
  format: yaml
  label: Grid Status Dataset Updates API
  slug: gridstatus-dataset-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-dataset-updates-api-openapi.yml
- filename: gridstatus-pricing-locations-api-openapi.yml
  format: yaml
  label: Grid Status Pricing Locations API
  slug: gridstatus-pricing-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-pricing-locations-api-openapi.yml
- filename: gridstatus-query-data-api-openapi.yml
  format: yaml
  label: Grid Status Query Data API
  slug: gridstatus-query-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-query-data-api-openapi.yml
- filename: gridstatus-reports-api-openapi.yml
  format: yaml
  label: Grid Status Reports API
  slug: gridstatus-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/openapi/gridstatus-reports-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gridstatus.io
  spf: true
hosts:
- cert_expires: Sep 11 14:26:52 2026 GMT
  host: www.gridstatus.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 05:09:00 2026 GMT
  host: docs.gridstatus.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 04:47:55 2026 GMT
  host: api.gridstatus.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gridstatus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grid Status, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Grid Status
provider_slug: gridstatus
slug: gridstatus-domain-security
source_filename: gridstatus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gridstatus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:26:52 2026 GMT\n  hsts: null\n- host: docs.gridstatus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:09:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gridstatus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 04:47:55 2026 GMT\n  hsts: null\ndomains:\n- domain: gridstatus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridstatus/refs/heads/main/security/gridstatus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Day-Ahead Prices
- Electricity
- Grid Data
- Energy Markets
- LMP
- Load
- Fuel Mix
- Open Source
---
