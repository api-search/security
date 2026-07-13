---
api_specs:
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Thermostat API
  slug: ecobee-thermostat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Thermostat Update and Functions API
  slug: ecobee-thermostat-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Runtime Report API
  slug: ecobee-runtime-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Group API
  slug: ecobee-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Demand Response API
  slug: ecobee-demand-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Hierarchy API
  slug: ecobee-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Meter Report API
  slug: ecobee-meter-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Authorization API
  slug: ecobee-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "sectigo.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecobee.com
  spf: true
hosts:
- cert_expires: Sep 23 16:21:16 2026 GMT
  host: www.ecobee.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 15:31:20 2027 GMT
  host: api.ecobee.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecobee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ecobee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ecobee
provider_slug: ecobee
slug: ecobee-domain-security
source_filename: ecobee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecobee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:21:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ecobee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 15:31:20 2027 GMT\n  hsts: null\ndomains:\n- domain: ecobee.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/security/ecobee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Smart Home
- Thermostat
- IoT
- HVAC
- Energy
- Home Automation
- Demand Response
---
