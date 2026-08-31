---
api_specs:
- filename: edf-energy-account-import-api-openapi.yml
  format: yaml
  label: EDF Energy Account Import API
  slug: edf-energy-account-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-account-import-api-openapi.yml
- filename: edf-energy-data-import-api-openapi.yml
  format: yaml
  label: EDF Energy Data Import API
  slug: edf-energy-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-data-import-api-openapi.yml
- filename: edf-energy-external-client-healthcheck-api-openapi.yml
  format: yaml
  label: EDF Energy External Client Healthcheck API
  slug: edf-energy-external-client-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-external-client-healthcheck-api-openapi.yml
- filename: edf-energy-external-events-api-openapi.yml
  format: yaml
  label: EDF Energy External Events API
  slug: edf-energy-external-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-external-events-api-openapi.yml
- filename: edf-energy-post-account-import-api-openapi.yml
  format: yaml
  label: EDF Energy Post Account Import API
  slug: edf-energy-post-account-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-post-account-import-api-openapi.yml
- filename: edf-energy-query-api-openapi.yml
  format: yaml
  label: EDF Energy Query API
  slug: edf-energy-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-query-api-openapi.yml
- filename: edf-energy-v1-api-openapi.yml
  format: yaml
  label: EDF Energy V1 API
  slug: edf-energy-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-v1-api-openapi.yml
- filename: edf-energy-v2-api-openapi.yml
  format: yaml
  label: EDF Energy V2 API
  slug: edf-energy-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-v2-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edfenergy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edfgb-kraken.energy
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.edfenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: developer.edfgb-kraken.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: api.edfgb-kraken.energy
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edf Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EDF Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EDF Energy
provider_slug: edf-energy
slug: edf-energy-domain-security
source_filename: edf-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.edfenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.edfgb-kraken.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.edfgb-kraken.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: edfenergy.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: edfgb-kraken.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/security/edf-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Retailer
- Energy Supplier
- Smart Metering
- Nuclear
- Renewables
- EV Charging
- Demand Response
- Tariffs
- Energy Markets
---
