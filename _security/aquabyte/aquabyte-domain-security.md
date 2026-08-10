---
api_specs:
- filename: aquabyte-behaviour-api-openapi.yml
  format: yaml
  label: Aquabyte Behaviour API
  slug: aquabyte-behaviour-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-behaviour-api-openapi.yml
- filename: aquabyte-biomass-api-openapi.yml
  format: yaml
  label: Aquabyte Biomass API
  slug: aquabyte-biomass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-biomass-api-openapi.yml
- filename: aquabyte-environmental-api-openapi.yml
  format: yaml
  label: Aquabyte Environmental API
  slug: aquabyte-environmental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-environmental-api-openapi.yml
- filename: aquabyte-lice-api-openapi.yml
  format: yaml
  label: Aquabyte Lice API
  slug: aquabyte-lice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-lice-api-openapi.yml
- filename: aquabyte-sites-api-openapi.yml
  format: yaml
  label: Aquabyte Sites API
  slug: aquabyte-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-sites-api-openapi.yml
- filename: aquabyte-v3-0-api-openapi.yml
  format: yaml
  label: Aquabyte V3.0 API
  slug: aquabyte-v3-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-v3-0-api-openapi.yml
- filename: aquabyte-welfare-api-openapi.yml
  format: yaml
  label: Aquabyte Welfare API
  slug: aquabyte-welfare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/openapi/aquabyte-welfare-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aquabyte.ai
  spf: true
hosts:
- cert_expires: Sep 19 03:31:50 2026 GMT
  host: www.aquabyte.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 01:05:35 2026 GMT
  host: api.aquabyte.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aquabyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aquabyte, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aquabyte
provider_slug: aquabyte
slug: aquabyte-domain-security
source_filename: aquabyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aquabyte.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.aquabyte.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:05:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: aquabyte.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aquabyte/refs/heads/main/security/aquabyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aquaculture
- Fish Farming
- Computer Vision
- Machine Learning
- Biomass Estimation
- Sea Lice
- Fish Welfare
- Environmental Monitoring
- Agriculture Technology
- Norway
- Salmon
- Data
---
