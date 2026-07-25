---
api_specs:
- filename: noaa-co-ops-benchmarks-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Benchmarks API
  slug: noaa-co-ops-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-benchmarks-api-openapi.yml
- filename: noaa-co-ops-datagetter-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Datagetter API
  slug: noaa-co-ops-datagetter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-datagetter-api-openapi.yml
- filename: noaa-co-ops-extremewaterlevels-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Extremewaterlevels API
  slug: noaa-co-ops-extremewaterlevels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-extremewaterlevels-api-openapi.yml
- filename: noaa-co-ops-htf-annual-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Htf Annual API
  slug: noaa-co-ops-htf-annual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-htf-annual-api-openapi.yml
- filename: noaa-co-ops-htf-monthly-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Htf Monthly API
  slug: noaa-co-ops-htf-monthly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-htf-monthly-api-openapi.yml
- filename: noaa-co-ops-htf-projection-decadal-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Htf Projection Decadal API
  slug: noaa-co-ops-htf-projection-decadal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-htf-projection-decadal-api-openapi.yml
- filename: noaa-co-ops-peakwaterlevels-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Peakwaterlevels API
  slug: noaa-co-ops-peakwaterlevels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-peakwaterlevels-api-openapi.yml
- filename: noaa-co-ops-ports-json-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Ports.json API
  slug: noaa-co-ops-ports-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-ports-json-api-openapi.yml
- filename: noaa-co-ops-sealvltrends-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Sealvltrends API
  slug: noaa-co-ops-sealvltrends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-sealvltrends-api-openapi.yml
- filename: noaa-co-ops-slr-projections-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Slr Projections API
  slug: noaa-co-ops-slr-projections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-slr-projections-api-openapi.yml
- filename: noaa-co-ops-stations-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Stations API
  slug: noaa-co-ops-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-stations-api-openapi.yml
- filename: noaa-co-ops-stations-json-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Stations.json API
  slug: noaa-co-ops-stations-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-stations-json-api-openapi.yml
- filename: noaa-co-ops-toptenwaterlevels-api-openapi.yml
  format: yaml
  label: NOAA CO-OPS Toptenwaterlevels API
  slug: noaa-co-ops-toptenwaterlevels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/noaa-co-ops-toptenwaterlevels-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: noaa.gov
  spf: true
hosts:
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: tidesandcurrents.noaa.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: api.tidesandcurrents.noaa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noaa Co Ops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NOAA CO-OPS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NOAA CO-OPS
provider_slug: noaa-co-ops
slug: noaa-co-ops-domain-security
source_filename: noaa-co-ops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tidesandcurrents.noaa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tidesandcurrents.noaa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: noaa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/security/noaa-co-ops-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- NOAA
- Tides
- Currents
- Oceanographic
- Water Level
- Weather
- Predictions
- Government
---
