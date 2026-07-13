---
api_specs:
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Pets API
  slug: digitail-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Pet Parents and Clients API
  slug: digitail-pet-parents-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Appointments API
  slug: digitail-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Clinical Records API
  slug: digitail-clinical-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Labs API
  slug: digitail-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Billing and Invoicing API
  slug: digitail-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Clinics and Staff API
  slug: digitail-clinics-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Client Communication API
  slug: digitail-client-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Files API
  slug: digitail-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
- filename: digitail-openapi.yml
  format: yaml
  label: Digitail Reports API
  slug: digitail-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/openapi/digitail-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: digitail.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: digitail.io
  spf: true
hosts:
- cert_expires: Sep 19 14:29:48 2026 GMT
  host: digitail.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 11:30:10 2026 GMT
  host: documentation.digitail.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 17:22:06 2026 GMT
  host: developer.digitail.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digitail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digitail, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Digitail
provider_slug: digitail
slug: digitail-domain-security
source_filename: digitail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 14:29:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documentation.digitail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:30:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.digitail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:22:06 2026 GMT\n  hsts: false\ndomains:\n- domain: digitail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: digitail.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digitail/refs/heads/main/security/digitail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Veterinary
- PIMS
- Practice Management
- Pets
- Healthcare
- Scheduling
- Billing
- SaaS
---
