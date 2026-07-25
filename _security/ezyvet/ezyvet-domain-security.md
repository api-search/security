---
api_specs:
- filename: ezyvet-animals-api-openapi.yml
  format: yaml
  label: ezyVet Animals API
  slug: ezyvet-animals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-animals-api-openapi.yml
- filename: ezyvet-appointments-api-openapi.yml
  format: yaml
  label: ezyVet Appointments API
  slug: ezyvet-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-appointments-api-openapi.yml
- filename: ezyvet-authentication-api-openapi.yml
  format: yaml
  label: ezyVet Authentication API
  slug: ezyvet-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-authentication-api-openapi.yml
- filename: ezyvet-consultations-api-openapi.yml
  format: yaml
  label: ezyVet Consultations API
  slug: ezyvet-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-consultations-api-openapi.yml
- filename: ezyvet-contacts-api-openapi.yml
  format: yaml
  label: ezyVet Contacts API
  slug: ezyvet-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-contacts-api-openapi.yml
- filename: ezyvet-diagnostics-api-openapi.yml
  format: yaml
  label: ezyVet Diagnostics API
  slug: ezyvet-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-diagnostics-api-openapi.yml
- filename: ezyvet-invoices-api-openapi.yml
  format: yaml
  label: ezyVet Invoices API
  slug: ezyvet-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-invoices-api-openapi.yml
- filename: ezyvet-prescriptions-api-openapi.yml
  format: yaml
  label: ezyVet Prescriptions API
  slug: ezyvet-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-prescriptions-api-openapi.yml
- filename: ezyvet-products-api-openapi.yml
  format: yaml
  label: ezyVet Products API
  slug: ezyvet-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ezyvet.com
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: www.ezyvet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: developers.ezyvet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.ezyvet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ezyvet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ezyVet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ezyVet
provider_slug: ezyvet
slug: ezyvet-domain-security
source_filename: ezyvet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ezyvet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.ezyvet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: false\n- host: api.ezyvet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ezyvet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/security/ezyvet-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Veterinary
- Practice Management
- PIMS
- Healthcare
- Animal Health
- IDEXX
- Partner Gated
---
