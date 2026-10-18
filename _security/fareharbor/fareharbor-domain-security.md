---
api_specs:
- filename: fareharbor-availabilities-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Availabilities Endpoints API
  slug: fareharbor-availabilities-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-availabilities-endpoints-api-openapi.yml
- filename: fareharbor-bookings-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Bookings Endpoints API
  slug: fareharbor-bookings-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-bookings-endpoints-api-openapi.yml
- filename: fareharbor-checkin-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Checkin Endpoints API
  slug: fareharbor-checkin-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-checkin-endpoints-api-openapi.yml
- filename: fareharbor-company-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Company Endpoints API
  slug: fareharbor-company-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-company-endpoints-api-openapi.yml
- filename: fareharbor-crew-members-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Crew Members Endpoints API
  slug: fareharbor-crew-members-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-crew-members-endpoints-api-openapi.yml
- filename: fareharbor-items-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Items Endpoints API
  slug: fareharbor-items-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-items-endpoints-api-openapi.yml
- filename: fareharbor-lodging-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Lodging Endpoints API
  slug: fareharbor-lodging-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-lodging-endpoints-api-openapi.yml
- filename: fareharbor-ping-api-openapi.yml
  format: yaml
  label: FareHarbor Ping API
  slug: fareharbor-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-ping-api-openapi.yml
- filename: fareharbor-roles-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Roles Endpoints API
  slug: fareharbor-roles-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-roles-endpoints-api-openapi.yml
- filename: fareharbor-users-endpoints-api-openapi.yml
  format: yaml
  label: FareHarbor Users Endpoints API
  slug: fareharbor-users-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/fareharbor-users-endpoints-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fareharbor.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: fareharbor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fareharbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FareHarbor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FareHarbor
provider_slug: fareharbor
slug: fareharbor-domain-security
source_filename: fareharbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fareharbor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fareharbor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/security/fareharbor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Booking
- Software-as-a-Service
- Tourism
- Software
---
