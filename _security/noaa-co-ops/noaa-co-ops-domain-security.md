---
api_specs:
- filename: data-retrieval-api.json
  format: json
  label: CO-OPS Data Retrieval API
  slug: co-ops-data-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/data-retrieval-api.json
- filename: metadata-api.json
  format: json
  label: CO-OPS Metadata API
  slug: co-ops-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/metadata-api.json
- filename: derived-product-api.json
  format: json
  label: CO-OPS Derived Product API
  slug: co-ops-derived-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noaa-co-ops/refs/heads/main/openapi/derived-product-api.json
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
