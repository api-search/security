---
api_specs:
- filename: solarwinds-orion-openapi.yml
  format: yaml
  label: SolarWinds Orion API
  slug: solarwinds-orion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-orion-openapi.yml
- filename: solarwinds-service-desk-openapi.yml
  format: yaml
  label: SolarWinds Service Desk API
  slug: solarwinds-service-desk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-service-desk-openapi.yml
- filename: openapi.json
  format: json
  label: SolarWinds Observability API
  slug: solarwinds-observability-api
  spec_type: OpenAPI
  url: https://api.na-01.cloud.solarwinds.com/v1/openapi.json
- filename: solarwinds-pingdom-openapi.yml
  format: yaml
  label: SolarWinds Pingdom API
  slug: solarwinds-pingdom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-pingdom-openapi.yml
- filename: solarwinds-loggly-openapi.yml
  format: yaml
  label: SolarWinds Loggly API
  slug: solarwinds-loggly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-loggly-openapi.yml
- filename: solarwinds-papertrail-openapi.yml
  format: yaml
  label: SolarWinds Papertrail API
  slug: solarwinds-papertrail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/openapi/solarwinds-papertrail-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: solarwinds.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pingdom.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.solarwinds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 01:27:54 2026 GMT
  host: api.na-01.cloud.solarwinds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 03:35:24 2026 GMT
  host: api.pingdom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solarwinds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SolarWinds, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SolarWinds
provider_slug: solarwinds
slug: solarwinds-domain-security
source_filename: solarwinds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solarwinds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.na-01.cloud.solarwinds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 01:27:54 2026 GMT\n  hsts: null\n- host: api.pingdom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:35:24 2026 GMT\n  hsts: null\ndomains:\n- domain: solarwinds.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pingdom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/security/solarwinds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Application Monitoring
- Database Monitoring
- Infrastructure
- IP Address Management
- IT Management
- ITSM
- Log Management
- Network Monitoring
- Observability
---
