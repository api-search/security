---
api_specs:
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Jobs API
  slug: servicem8-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Job Activities API
  slug: servicem8-job-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Clients (Companies) API
  slug: servicem8-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Job Contacts API
  slug: servicem8-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Staff API
  slug: servicem8-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Materials API
  slug: servicem8-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Attachments API
  slug: servicem8-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Queues API
  slug: servicem8-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Vendors API
  slug: servicem8-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Badges API
  slug: servicem8-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Webhooks API
  slug: servicem8-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: servicem8.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.servicem8.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: developer.servicem8.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.servicem8.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Servicem8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ServiceM8, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ServiceM8
provider_slug: servicem8
slug: servicem8-domain-security
source_filename: servicem8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.servicem8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.servicem8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n- host: api.servicem8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: servicem8.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/security/servicem8-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service
- Job Management
- Trades
- Scheduling
- Dispatch
- Invoicing
- Home Services
---
