---
api_specs:
- filename: us-geological-survey-collections-api-openapi.yml
  format: yaml
  label: US Geological Survey Collections API
  slug: us-geological-survey-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-collections-api-openapi.yml
- filename: us-geological-survey-continuous-values-api-openapi.yml
  format: yaml
  label: US Geological Survey Continuous Values API
  slug: us-geological-survey-continuous-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-continuous-values-api-openapi.yml
- filename: us-geological-survey-daily-values-api-openapi.yml
  format: yaml
  label: US Geological Survey Daily Values API
  slug: us-geological-survey-daily-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-daily-values-api-openapi.yml
- filename: us-geological-survey-earthquakes-api-openapi.yml
  format: yaml
  label: US Geological Survey Earthquakes API
  slug: us-geological-survey-earthquakes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-earthquakes-api-openapi.yml
- filename: us-geological-survey-field-measurements-api-openapi.yml
  format: yaml
  label: US Geological Survey Field Measurements API
  slug: us-geological-survey-field-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-field-measurements-api-openapi.yml
- filename: us-geological-survey-metadata-api-openapi.yml
  format: yaml
  label: US Geological Survey Metadata API
  slug: us-geological-survey-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-metadata-api-openapi.yml
- filename: us-geological-survey-monitoring-locations-api-openapi.yml
  format: yaml
  label: US Geological Survey Monitoring Locations API
  slug: us-geological-survey-monitoring-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-monitoring-locations-api-openapi.yml
- filename: us-geological-survey-time-series-metadata-api-openapi.yml
  format: yaml
  label: US Geological Survey Time Series Metadata API
  slug: us-geological-survey-time-series-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/openapi/us-geological-survey-time-series-metadata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usgs.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sciencebase.gov
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: earthquake.usgs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:20:52 2026 GMT
  host: api.waterdata.usgs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.sciencebase.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Geological Survey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Geological Survey, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Geological Survey
provider_slug: us-geological-survey
slug: us-geological-survey-domain-security
source_filename: us-geological-survey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earthquake.usgs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.waterdata.usgs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:20:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.sciencebase.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usgs.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sciencebase.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-geological-survey/refs/heads/main/security/us-geological-survey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Earth Science
- Earthquakes
- Water Data
- Geospatial
- Hazards
- Environment
---
