---
api_specs:
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Authentication API
  slug: spike-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Provider Integrations API
  slug: spike-api-provider-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Provider Records API
  slug: spike-api-provider-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Sleep API
  slug: spike-api-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Workouts API
  slug: spike-api-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Time Series API
  slug: spike-api-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Statistics API
  slug: spike-api-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Nutrition AI API
  slug: spike-api-nutrition-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Lab Reports API
  slug: spike-api-lab-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike Users API
  slug: spike-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
- filename: spike-api-openapi.yml
  format: yaml
  label: Spike SDK Push API
  slug: spike-api-sdk-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/openapi/spike-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spikeapi.com
  spf: true
hosts:
- cert_expires: Sep 25 00:21:42 2026 GMT
  host: www.spikeapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 11:32:38 2026 GMT
  host: docs.spikeapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: app-api.spikeapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spike Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spike, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spike
provider_slug: spike-api
slug: spike-api-domain-security
source_filename: spike-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spikeapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:21:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.spikeapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:32:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app-api.spikeapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: spikeapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spike-api/refs/heads/main/security/spike-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health Data
- Wearables
- Fitness
- Digital Health
- Data Aggregation
- HIPAA
---
