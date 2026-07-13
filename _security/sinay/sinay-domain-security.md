---
api_specs:
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Ports and Vessels API
  slug: sinay-ports-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Metocean API
  slug: sinay-metocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay CO2 Emission API
  slug: sinay-co2-emission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay ETA API
  slug: sinay-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
- filename: sinay-openapi.yml
  format: yaml
  label: Sinay Port Congestion API
  slug: sinay-port-congestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/openapi/sinay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: none
  dnssec: false
  domain: sinay.ai
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com ~all
hosts:
- cert_expires: Aug 22 11:59:45 2026 GMT
  host: sinay.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 11:59:45 2026 GMT
  host: api.sinay.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sinay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sinay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent (p=none).'
provider_name: Sinay
provider_slug: sinay
slug: sinay-domain-security
source_filename: sinay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sinay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:59:45 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.sinay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:59:45 2026 GMT\n  hsts: false\ndomains:\n- domain: sinay.ai\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.protection.outlook.com ~all'\n  dmarc: false\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinay/refs/heads/main/security/sinay-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Vessel Tracking
- AIS
- Maritime
- Maritime Data
- Weather
- CO2 Emissions
- Port Congestion
- Ship Tracking
- ETA
- Ocean Data
---
