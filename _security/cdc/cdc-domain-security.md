---
api_specs:
- filename: cdc-app-notifications-api-openapi.yml
  format: yaml
  label: CDC app-notifications API
  slug: cdc-app-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-app-notifications-api-openapi.yml
- filename: cdc-code-systems-api-openapi.yml
  format: yaml
  label: CDC code-systems API
  slug: cdc-code-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-code-systems-api-openapi.yml
- filename: cdc-conditions-api-openapi.yml
  format: yaml
  label: CDC conditions API
  slug: cdc-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-conditions-api-openapi.yml
- filename: cdc-configurations-api-openapi.yml
  format: yaml
  label: CDC configurations API
  slug: cdc-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-configurations-api-openapi.yml
- filename: cdc-events-api-openapi.yml
  format: yaml
  label: CDC events API
  slug: cdc-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-events-api-openapi.yml
- filename: cdc-query-api-openapi.yml
  format: yaml
  label: CDC Query API
  slug: cdc-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-query-api-openapi.yml
- filename: cdc-query-connector-api-openapi-3-0-api-openapi.yml
  format: yaml
  label: CDC Query Connector API OpenAPI 3.0 API
  slug: cdc-query-connector-api-openapi-3-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-query-connector-api-openapi-3-0-api-openapi.yml
- filename: cdc-releases-api-openapi.yml
  format: yaml
  label: CDC releases API
  slug: cdc-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-releases-api-openapi.yml
- filename: cdc-simulator-api-openapi.yml
  format: yaml
  label: CDC simulator API
  slug: cdc-simulator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-simulator-api-openapi.yml
- filename: cdc-user-api-openapi.yml
  format: yaml
  label: CDC user API
  slug: cdc-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/cdc-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cdc.gov
  spf: true
hosts:
- host: open.cdc.gov
  https: false
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: data.cdc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 28 13:32:05 2026 GMT
  host: wonder.cdc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cdc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CDC, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CDC
provider_slug: cdc
slug: cdc-domain-security
source_filename: cdc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.cdc.gov\n  https: false\n- host: data.cdc.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wonder.cdc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:32:05 2026 GMT\n  hsts: null\ndomains:\n- domain: cdc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/security/cdc-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Public Health
- Disease Surveillance
- Vaccination
- Health Statistics
- Government
- Open Data
- Environmental Health
- Mortality
- CDC WONDER
---
