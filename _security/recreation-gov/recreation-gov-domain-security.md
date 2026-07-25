---
api_specs:
- filename: recreation-gov-activities-api-openapi.yml
  format: yaml
  label: Recreation.gov Activities API
  slug: recreation-gov-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-activities-api-openapi.yml
- filename: recreation-gov-campsites-api-openapi.yml
  format: yaml
  label: Recreation.gov Campsites API
  slug: recreation-gov-campsites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-campsites-api-openapi.yml
- filename: recreation-gov-events-api-openapi.yml
  format: yaml
  label: Recreation.gov Events API
  slug: recreation-gov-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-events-api-openapi.yml
- filename: recreation-gov-facilities-api-openapi.yml
  format: yaml
  label: Recreation.gov Facilities API
  slug: recreation-gov-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-facilities-api-openapi.yml
- filename: recreation-gov-links-api-openapi.yml
  format: yaml
  label: Recreation.gov Links API
  slug: recreation-gov-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-links-api-openapi.yml
- filename: recreation-gov-media-api-openapi.yml
  format: yaml
  label: Recreation.gov Media API
  slug: recreation-gov-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-media-api-openapi.yml
- filename: recreation-gov-organizations-api-openapi.yml
  format: yaml
  label: Recreation.gov Organizations API
  slug: recreation-gov-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-organizations-api-openapi.yml
- filename: recreation-gov-permitentrances-api-openapi.yml
  format: yaml
  label: Recreation.gov Permitentrances API
  slug: recreation-gov-permitentrances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-permitentrances-api-openapi.yml
- filename: recreation-gov-recareas-api-openapi.yml
  format: yaml
  label: Recreation.gov Recareas API
  slug: recreation-gov-recareas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-recareas-api-openapi.yml
- filename: recreation-gov-tours-api-openapi.yml
  format: yaml
  label: Recreation.gov Tours API
  slug: recreation-gov-tours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/openapi/recreation-gov-tours-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: recreation.gov
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.recreation.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: ridb.recreation.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recreation Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recreation.gov, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Recreation.gov
provider_slug: recreation-gov
slug: recreation-gov-domain-security
source_filename: recreation-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.recreation.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ridb.recreation.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: recreation.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recreation-gov/refs/heads/main/security/recreation-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Recreation
- Federal
- Camping
- Outdoors
- Public Lands
---
