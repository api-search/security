---
api_specs:
- filename: utilityapi-accounting-api-openapi.yml
  format: yaml
  label: UtilityAPI Accounting API
  slug: utilityapi-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-accounting-api-openapi.yml
- filename: utilityapi-authorizations-api-openapi.yml
  format: yaml
  label: UtilityAPI Authorizations API
  slug: utilityapi-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-authorizations-api-openapi.yml
- filename: utilityapi-bills-api-openapi.yml
  format: yaml
  label: UtilityAPI Bills API
  slug: utilityapi-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-bills-api-openapi.yml
- filename: utilityapi-events-api-openapi.yml
  format: yaml
  label: UtilityAPI Events API
  slug: utilityapi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-events-api-openapi.yml
- filename: utilityapi-files-api-openapi.yml
  format: yaml
  label: UtilityAPI Files API
  slug: utilityapi-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-files-api-openapi.yml
- filename: utilityapi-forms-api-openapi.yml
  format: yaml
  label: UtilityAPI Forms API
  slug: utilityapi-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-forms-api-openapi.yml
- filename: utilityapi-intervals-api-openapi.yml
  format: yaml
  label: UtilityAPI Intervals API
  slug: utilityapi-intervals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-intervals-api-openapi.yml
- filename: utilityapi-meters-api-openapi.yml
  format: yaml
  label: UtilityAPI Meters API
  slug: utilityapi-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-meters-api-openapi.yml
- filename: utilityapi-templates-api-openapi.yml
  format: yaml
  label: UtilityAPI Templates API
  slug: utilityapi-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/openapi/utilityapi-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: utilityapi.com
  spf: true
hosts:
- cert_expires: Aug 17 19:11:25 2026 GMT
  host: utilityapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Utilityapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UtilityAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UtilityAPI
provider_slug: utilityapi
slug: utilityapi-domain-security
source_filename: utilityapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utilityapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:11:25 2026 GMT\n  hsts: false\ndomains:\n- domain: utilityapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utilityapi/refs/heads/main/security/utilityapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Utilities
- Green Button
- Billing Data
- Meter Data
- Clean Energy
---
