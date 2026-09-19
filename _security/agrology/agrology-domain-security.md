---
api_specs:
- filename: agrology-alerts-api-openapi.yml
  format: yaml
  label: Agrology Alerts API
  slug: agrology-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-alerts-api-openapi.yml
- filename: agrology-charts-api-openapi.yml
  format: yaml
  label: Agrology Charts API
  slug: agrology-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-charts-api-openapi.yml
- filename: agrology-dashboards-api-openapi.yml
  format: yaml
  label: Agrology Dashboards API
  slug: agrology-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-dashboards-api-openapi.yml
- filename: agrology-experiments-api-openapi.yml
  format: yaml
  label: Agrology Experiments API
  slug: agrology-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-experiments-api-openapi.yml
- filename: agrology-feedback-api-openapi.yml
  format: yaml
  label: Agrology Feedback API
  slug: agrology-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-feedback-api-openapi.yml
- filename: agrology-files-api-openapi.yml
  format: yaml
  label: Agrology Files API
  slug: agrology-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-files-api-openapi.yml
- filename: agrology-ground-truth-api-openapi.yml
  format: yaml
  label: Agrology Ground Truth API
  slug: agrology-ground-truth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-ground-truth-api-openapi.yml
- filename: agrology-metrics-api-openapi.yml
  format: yaml
  label: Agrology Metrics API
  slug: agrology-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-metrics-api-openapi.yml
- filename: agrology-microclimate-api-openapi.yml
  format: yaml
  label: Agrology Microclimate API
  slug: agrology-microclimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-microclimate-api-openapi.yml
- filename: agrology-reports-api-openapi.yml
  format: yaml
  label: Agrology Reports API
  slug: agrology-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-reports-api-openapi.yml
- filename: agrology-summary-data-api-openapi.yml
  format: yaml
  label: Agrology Summary Data API
  slug: agrology-summary-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-summary-data-api-openapi.yml
- filename: agrology-synthetics-api-openapi.yml
  format: yaml
  label: Agrology Synthetics API
  slug: agrology-synthetics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-synthetics-api-openapi.yml
- filename: agrology-topology-api-openapi.yml
  format: yaml
  label: Agrology Topology API
  slug: agrology-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-topology-api-openapi.yml
- filename: agrology-user-api-openapi.yml
  format: yaml
  label: Agrology User API
  slug: agrology-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-user-api-openapi.yml
- filename: agrology-weather-api-openapi.yml
  format: yaml
  label: Agrology Weather API
  slug: agrology-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agrology.ag
  spf: true
hosts:
- cert_expires: Oct 22 15:53:54 2026 GMT
  host: agrology.ag
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api.agrology.ag
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agrology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agrology, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agrology
provider_slug: agrology
slug: agrology-domain-security
source_filename: agrology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agrology.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 15:53:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.agrology.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: agrology.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/security/agrology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- AgTech
- Climate
- Sensors
- IoT
- Weather
- Soil
- Carbon
- Predictive Analytics
- Geospatial
- Time Series
- Machine-Learning
- Viticulture
- Sustainability
- Environmental Monitoring
---
