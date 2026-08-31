---
api_specs:
- filename: inrix-accounts-api-openapi.yml
  format: yaml
  label: INRIX Accounts API
  slug: inrix-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-accounts-api-openapi.yml
- filename: inrix-api-api-openapi.yml
  format: yaml
  label: INRIX API
  slug: inrix-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-api-api-openapi.yml
- filename: inrix-application-api-openapi.yml
  format: yaml
  label: INRIX Application API
  slug: inrix-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-application-api-openapi.yml
- filename: inrix-applicationmanagement-api-openapi.yml
  format: yaml
  label: INRIX Application Management API
  slug: inrix-applicationmanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-applicationmanagement-api-openapi.yml
- filename: inrix-auth-api-openapi.yml
  format: yaml
  label: INRIX Auth API
  slug: inrix-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-auth-api-openapi.yml
- filename: inrix-developer-api-openapi.yml
  format: yaml
  label: INRIX Developer API
  slug: inrix-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-developer-api-openapi.yml
- filename: inrix-device-api-openapi.yml
  format: yaml
  label: INRIX Device API
  slug: inrix-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-device-api-openapi.yml
- filename: inrix-emailtemplate-api-openapi.yml
  format: yaml
  label: INRIX Email Template API
  slug: inrix-emailtemplate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-emailtemplate-api-openapi.yml
- filename: inrix-metadata-api-openapi.yml
  format: yaml
  label: INRIX Metadata API
  slug: inrix-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-metadata-api-openapi.yml
- filename: inrix-metrics-api-openapi.yml
  format: yaml
  label: INRIX Metrics API
  slug: inrix-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-metrics-api-openapi.yml
- filename: inrix-namespace-management-api-openapi.yml
  format: yaml
  label: INRIX Namespace Management API
  slug: inrix-namespace-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-namespace-management-api-openapi.yml
- filename: inrix-user-api-openapi.yml
  format: yaml
  label: INRIX User API
  slug: inrix-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-user-api-openapi.yml
- filename: inrix-usergroup-api-openapi.yml
  format: yaml
  label: INRIX User Group API
  slug: inrix-usergroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-usergroup-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inrix.com
  spf: true
hosts:
- cert_expires: Oct 12 11:10:55 2026 GMT
  host: inrix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: docs.inrix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: uas-api.inrix.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Inrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INRIX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: INRIX
provider_slug: inrix
slug: inrix-domain-security
source_filename: inrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:10:55 2026 GMT\n  hsts: null\n- host: docs.inrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\n- host: uas-api.inrix.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: inrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/security/inrix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Traffic
- Mobility
- Parking
- Geospatial
- Location Data
- Analytics
- Automotive
- Smart Cities
- Routing
- Connected Vehicles
- Road Network
- Data
- Fleet
- Intelligent Transportation Systems
---
