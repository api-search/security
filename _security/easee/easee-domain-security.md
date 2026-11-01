---
api_specs:
- filename: easee-account-api-openapi.yml
  format: yaml
  label: Easee Account API
  slug: easee-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-account-api-openapi.yml
- filename: easee-authorizecharging-api-openapi.yml
  format: yaml
  label: Easee Authorize Charging API
  slug: easee-authorizecharging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-authorizecharging-api-openapi.yml
- filename: easee-charge-session-api-openapi.yml
  format: yaml
  label: Easee Charge Session API
  slug: easee-charge-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-charge-session-api-openapi.yml
- filename: easee-charger-api-openapi.yml
  format: yaml
  label: Easee Charger API
  slug: easee-charger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-charger-api-openapi.yml
- filename: easee-cloud-ocpp-api-openapi.yml
  format: yaml
  label: Easee Cloud OCPP API
  slug: easee-cloud-ocpp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-cloud-ocpp-api-openapi.yml
- filename: easee-daily-schedule-api-openapi.yml
  format: yaml
  label: Easee Daily schedule API
  slug: easee-daily-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-daily-schedule-api-openapi.yml
- filename: easee-delayed-schedule-api-openapi.yml
  format: yaml
  label: Easee Delayed schedule API
  slug: easee-delayed-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-delayed-schedule-api-openapi.yml
- filename: easee-direct-ocpp-for-operators-api-openapi.yml
  format: yaml
  label: Easee Direct OCPP - For Operators API
  slug: easee-direct-ocpp-for-operators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-direct-ocpp-for-operators-api-openapi.yml
- filename: easee-direct-ocpp-for-users-api-openapi.yml
  format: yaml
  label: Easee Direct OCPP - For Users API
  slug: easee-direct-ocpp-for-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-direct-ocpp-for-users-api-openapi.yml
- filename: easee-easeekeys-api-openapi.yml
  format: yaml
  label: Easee Easee Keys API
  slug: easee-easeekeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-easeekeys-api-openapi.yml
- filename: easee-energy-reporting-api-openapi.yml
  format: yaml
  label: Easee Energy Reporting API
  slug: easee-energy-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-energy-reporting-api-openapi.yml
- filename: easee-equalizer-api-openapi.yml
  format: yaml
  label: Easee Equalizer API
  slug: easee-equalizer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-equalizer-api-openapi.yml
- filename: easee-observations-api-openapi.yml
  format: yaml
  label: Easee Observations API
  slug: easee-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-observations-api-openapi.yml
- filename: easee-resources-api-openapi.yml
  format: yaml
  label: Easee Resources API
  slug: easee-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-resources-api-openapi.yml
- filename: easee-site-api-openapi.yml
  format: yaml
  label: Easee Site API
  slug: easee-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-site-api-openapi.yml
- filename: easee-site-charge-session-api-openapi.yml
  format: yaml
  label: Easee Site Charge Session API
  slug: easee-site-charge-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-site-charge-session-api-openapi.yml
- filename: easee-state-api-openapi.yml
  format: yaml
  label: Easee State API
  slug: easee-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-state-api-openapi.yml
- filename: easee-weekly-schedule-api-openapi.yml
  format: yaml
  label: Easee Weekly schedule API
  slug: easee-weekly-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-weekly-schedule-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: easee.com
  spf: true
hosts:
- cert_expires: Dec 21 12:31:32 2026 GMT
  host: easee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Easee
provider_slug: easee
slug: easee-domain-security
source_filename: easee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 12:31:32 2026 GMT\n  hsts: false\ndomains:\n- domain: easee.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/easee/security/easee-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- EVCharging
- SmartHome
- IoT
- Energy
---
