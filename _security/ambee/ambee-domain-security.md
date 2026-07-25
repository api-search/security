---
api_specs:
- filename: ambee-air-quality-api-openapi.yml
  format: yaml
  label: Ambee Air Quality API
  slug: ambee-air-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-air-quality-api-openapi.yml
- filename: ambee-fire-api-openapi.yml
  format: yaml
  label: Ambee Fire API
  slug: ambee-fire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-fire-api-openapi.yml
- filename: ambee-ndvi-api-openapi.yml
  format: yaml
  label: Ambee NDVI API
  slug: ambee-ndvi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-ndvi-api-openapi.yml
- filename: ambee-pollen-api-openapi.yml
  format: yaml
  label: Ambee Pollen API
  slug: ambee-pollen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-pollen-api-openapi.yml
- filename: ambee-soil-api-openapi.yml
  format: yaml
  label: Ambee Soil API
  slug: ambee-soil-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-soil-api-openapi.yml
- filename: ambee-weather-api-openapi.yml
  format: yaml
  label: Ambee Weather API
  slug: ambee-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/openapi/ambee-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getambee.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ambeedata.com
  spf: false
hosts:
- cert_expires: Sep 30 01:45:30 2026 GMT
  host: www.getambee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: api.ambeedata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambee, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ambee
provider_slug: ambee
slug: ambee-domain-security
source_filename: ambee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getambee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:45:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ambeedata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: getambee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ambeedata.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambee/refs/heads/main/security/ambee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Environmental Intelligence
- Air Quality
- Weather
- Pollen
- Geospatial
---
