---
api_specs:
- filename: atmospore-pollen-forecasts-pollen-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen API
  slug: atmospore-pollen-forecasts-pollen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-api-openapi.yml
- filename: atmospore-pollen-forecasts-pollen-area-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen Area API
  slug: atmospore-pollen-forecasts-pollen-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-area-api-openapi.yml
- filename: atmospore-pollen-forecasts-pollen-top-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Pollen Top API
  slug: atmospore-pollen-forecasts-pollen-top-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-pollen-top-api-openapi.yml
- filename: atmospore-pollen-forecasts-species-api-openapi.yml
  format: yaml
  label: Atmospore Pollen Forecasts Species API
  slug: atmospore-pollen-forecasts-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/openapi/atmospore-pollen-forecasts-species-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atmospore.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pollenapi.com
  spf: false
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: atmospore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: pollenapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atmospore Pollen Forecasts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmospore Pollen Forecasts, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atmospore Pollen Forecasts
provider_slug: atmospore-pollen-forecasts
slug: atmospore-pollen-forecasts-domain-security
source_filename: atmospore-pollen-forecasts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atmospore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\n- host: pollenapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: atmospore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pollenapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmospore-pollen-forecasts/refs/heads/main/security/atmospore-pollen-forecasts-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Pollen
- Allergy
- Environmental Data
- Health
- Geospatial
- Forecasting
- Smart Home
- MCP
- OpenAPI
- Norway
- Climate
---
