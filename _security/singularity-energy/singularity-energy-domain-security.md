---
api_specs:
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Carbon Intensity API
  slug: carbon-intensity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Forecasts API
  slug: forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Generation & Event Data API
  slug: generation-event-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Regions API
  slug: regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: singularity.energy
  spf: true
hosts:
- cert_expires: Oct  3 23:55:17 2026 GMT
  host: www.singularity.energy
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 06:04:09 2026 GMT
  host: docs.singularity.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: api.singularity.energy
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Singularity Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Singularity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Singularity
provider_slug: singularity-energy
slug: singularity-energy-domain-security
source_filename: singularity-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.singularity.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:55:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.singularity.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:04:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.singularity.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: singularity.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/security/singularity-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Carbon Emissions
- Grid
- Sustainability
- Carbon Intensity
---
