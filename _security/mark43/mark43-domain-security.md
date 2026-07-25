---
api_specs:
- filename: mark43-associated-records-api-openapi.yml
  format: yaml
  label: Mark43 Associated Records API
  slug: mark43-associated-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-associated-records-api-openapi.yml
- filename: mark43-attachments-api-openapi.yml
  format: yaml
  label: Mark43 Attachments API
  slug: mark43-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-attachments-api-openapi.yml
- filename: mark43-cad-configuration-api-openapi.yml
  format: yaml
  label: Mark43 CAD Configuration API
  slug: mark43-cad-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-cad-configuration-api-openapi.yml
- filename: mark43-cad-events-api-openapi.yml
  format: yaml
  label: Mark43 CAD Events API
  slug: mark43-cad-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-cad-events-api-openapi.yml
- filename: mark43-cad-tickets-api-openapi.yml
  format: yaml
  label: Mark43 CAD Tickets API
  slug: mark43-cad-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-cad-tickets-api-openapi.yml
- filename: mark43-cases-api-openapi.yml
  format: yaml
  label: Mark43 Cases API
  slug: mark43-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-cases-api-openapi.yml
- filename: mark43-e911-api-openapi.yml
  format: yaml
  label: Mark43 E911 API
  slug: mark43-e911-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-e911-api-openapi.yml
- filename: mark43-evidence-api-openapi.yml
  format: yaml
  label: Mark43 Evidence API
  slug: mark43-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-evidence-api-openapi.yml
- filename: mark43-gps-api-openapi.yml
  format: yaml
  label: Mark43 GPS API
  slug: mark43-gps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-gps-api-openapi.yml
- filename: mark43-persons-api-openapi.yml
  format: yaml
  label: Mark43 Persons API
  slug: mark43-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-persons-api-openapi.yml
- filename: mark43-reports-api-openapi.yml
  format: yaml
  label: Mark43 Reports API
  slug: mark43-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-reports-api-openapi.yml
- filename: mark43-tasks-api-openapi.yml
  format: yaml
  label: Mark43 Tasks API
  slug: mark43-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-tasks-api-openapi.yml
- filename: mark43-users-api-openapi.yml
  format: yaml
  label: Mark43 Users API
  slug: mark43-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-users-api-openapi.yml
- filename: mark43-vehicles-api-openapi.yml
  format: yaml
  label: Mark43 Vehicles API
  slug: mark43-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-vehicles-api-openapi.yml
- filename: mark43-warrants-api-openapi.yml
  format: yaml
  label: Mark43 Warrants API
  slug: mark43-warrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/openapi/mark43-warrants-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mark43.com
  spf: true
hosts:
- cert_expires: Oct  9 22:07:34 2026 GMT
  host: mark43.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: developers.mark43.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: department.mark43.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mark43 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mark43, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mark43
provider_slug: mark43
slug: mark43-domain-security
source_filename: mark43-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mark43.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 22:07:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.mark43.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n- host: department.mark43.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: mark43.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mark43/refs/heads/main/security/mark43-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Public Safety
- Law Enforcement
- Records Management
- Computer-Aided Dispatch
- CAD
- RMS
- GovTech
- Evidence Management
- Government
---
