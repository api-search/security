---
api_specs:
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Authentication API
  slug: ezyvet-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Animals (Patients) API
  slug: ezyvet-animals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Contacts (Clients) API
  slug: ezyvet-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Appointments API
  slug: ezyvet-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Consultations (Clinical) API
  slug: ezyvet-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Invoices (Billing) API
  slug: ezyvet-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Products (Inventory) API
  slug: ezyvet-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Diagnostics API
  slug: ezyvet-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
- filename: ezyvet-openapi.yml
  format: yaml
  label: ezyVet Prescriptions and Vaccinations API
  slug: ezyvet-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezyvet/refs/heads/main/openapi/ezyvet-openapi.yml
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
