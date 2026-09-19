---
api_specs:
- filename: cheniere-energy-capacity-api-openapi.yml
  format: yaml
  label: Cheniere Energy Capacity API
  slug: cheniere-energy-capacity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-capacity-api-openapi.yml
- filename: cheniere-energy-discovery-api-openapi.yml
  format: yaml
  label: Cheniere Energy Discovery API
  slug: cheniere-energy-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-discovery-api-openapi.yml
- filename: cheniere-energy-documents-api-openapi.yml
  format: yaml
  label: Cheniere Energy Documents API
  slug: cheniere-energy-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-documents-api-openapi.yml
- filename: cheniere-energy-gas-quality-api-openapi.yml
  format: yaml
  label: Cheniere Energy Gas Quality API
  slug: cheniere-energy-gas-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-gas-quality-api-openapi.yml
- filename: cheniere-energy-imbalances-api-openapi.yml
  format: yaml
  label: Cheniere Energy Imbalances API
  slug: cheniere-energy-imbalances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-imbalances-api-openapi.yml
- filename: cheniere-energy-index-of-customers-api-openapi.yml
  format: yaml
  label: Cheniere Energy Index of Customers API
  slug: cheniere-energy-index-of-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-index-of-customers-api-openapi.yml
- filename: cheniere-energy-notices-api-openapi.yml
  format: yaml
  label: Cheniere Energy Notices API
  slug: cheniere-energy-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-notices-api-openapi.yml
- filename: cheniere-energy-reference-data-api-openapi.yml
  format: yaml
  label: Cheniere Energy Reference Data API
  slug: cheniere-energy-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-reference-data-api-openapi.yml
- filename: cheniere-energy-telemetry-api-openapi.yml
  format: yaml
  label: Cheniere Energy Telemetry API
  slug: cheniere-energy-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-telemetry-api-openapi.yml
- filename: cheniere-energy-transactional-reporting-api-openapi.yml
  format: yaml
  label: Cheniere Energy Transactional Reporting API
  slug: cheniere-energy-transactional-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/openapi/cheniere-energy-transactional-reporting-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cheniere.com
  spf: true
hosts:
- cert_expires: Nov 15 08:05:24 2026 GMT
  host: www.cheniere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: lngconnection.cheniere.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: lngconnectionapi.cheniere.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cheniere Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cheniere Energy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cheniere Energy
provider_slug: cheniere-energy
slug: cheniere-energy-domain-security
source_filename: cheniere-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cheniere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 08:05:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: lngconnection.cheniere.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: lngconnectionapi.cheniere.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cheniere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheniere-energy/refs/heads/main/security/cheniere-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corpus Christi
- Energy
- Export
- FERC
- Houston
- Informational Postings
- LNG
- Liquefaction
- NAESB
- Natural Gas
- Open Data
- Pipelines
- Regasification
- Sabine Pass
- Texas
---
