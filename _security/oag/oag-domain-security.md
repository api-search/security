---
api_specs:
- filename: oag-alerts-api-openapi.yml
  format: yaml
  label: OAG Alerts API
  slug: oag-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-alerts-api-openapi.yml
- filename: oag-flight-connections-api-openapi.yml
  format: yaml
  label: OAG Flight Connections API
  slug: oag-flight-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-flight-connections-api-openapi.yml
- filename: oag-flight-info-alerts-api-openapi.yml
  format: yaml
  label: OAG Flight Info Alerts API
  slug: oag-flight-info-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-flight-info-alerts-api-openapi.yml
- filename: oag-flight-instances-api-openapi.yml
  format: yaml
  label: OAG Flight Instances API
  slug: oag-flight-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-flight-instances-api-openapi.yml
- filename: oag-flights-api-openapi.yml
  format: yaml
  label: OAG Flights API
  slug: oag-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-flights-api-openapi.yml
- filename: oag-locations-api-openapi.yml
  format: yaml
  label: OAG Locations API
  slug: oag-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-locations-api-openapi.yml
- filename: oag-oag-api-api-openapi.yml
  format: yaml
  label: OAG OAG API
  slug: oag-oag-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-oag-api-api-openapi.yml
- filename: oag-profile-api-openapi.yml
  format: yaml
  label: OAG Profile API
  slug: oag-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-profile-api-openapi.yml
- filename: oag-status-api-openapi.yml
  format: yaml
  label: OAG Status API
  slug: oag-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/openapi/oag-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oag.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: oag.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OAG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OAG
provider_slug: oag
slug: oag-domain-security
source_filename: oag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oag.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oag/refs/heads/main/security/oag-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Aviation
- Data
- Analytics
- Travel
---
