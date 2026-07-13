---
api_specs:
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Access Token API
  slug: vagaro-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Appointments API
  slug: vagaro-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Customers API
  slug: vagaro-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Employees API
  slug: vagaro-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Employee Management API
  slug: vagaro-employee-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
- filename: vagaro-openapi.yml
  format: yaml
  label: Vagaro Locations API
  slug: vagaro-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/openapi/vagaro-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vagaro.com
  spf: true
hosts:
- cert_expires: Sep 30 14:29:29 2026 GMT
  host: www.vagaro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 03:17:40 2026 GMT
  host: docs.vagaro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:29:29 2026 GMT
  host: api.vagaro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vagaro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vagaro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vagaro
provider_slug: vagaro
slug: vagaro-domain-security
source_filename: vagaro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vagaro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:29:29 2026 GMT\n  hsts: null\n- host: docs.vagaro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:17:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vagaro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:29:29 2026 GMT\n  hsts: null\ndomains:\n- domain: vagaro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vagaro/refs/heads/main/security/vagaro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Salon
- Spa
- Fitness
- Wellness
- Scheduling
- Booking
- Vertical SaaS
---
