---
api_specs:
- filename: fieldwire-account-api-openapi.yml
  format: yaml
  label: Fieldwire Account API
  slug: fieldwire-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-account-api-openapi.yml
- filename: fieldwire-projects-api-openapi.yml
  format: yaml
  label: Fieldwire Projects API
  slug: fieldwire-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-projects-api-openapi.yml
- filename: fieldwire-tasks-api-openapi.yml
  format: yaml
  label: Fieldwire Tasks API
  slug: fieldwire-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-tasks-api-openapi.yml
- filename: fieldwire-plans-api-openapi.yml
  format: yaml
  label: Fieldwire Plans and Sheets API
  slug: fieldwire-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-plans-api-openapi.yml
- filename: fieldwire-forms-api-openapi.yml
  format: yaml
  label: Fieldwire Forms API
  slug: fieldwire-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-forms-api-openapi.yml
- filename: fieldwire-attachments-api-openapi.yml
  format: yaml
  label: Fieldwire Attachments and Media API
  slug: fieldwire-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-attachments-api-openapi.yml
- filename: fieldwire-financials-api-openapi.yml
  format: yaml
  label: Fieldwire Project Financials API
  slug: fieldwire-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-financials-api-openapi.yml
- filename: fieldwire-rfis-submittals-api-openapi.yml
  format: yaml
  label: Fieldwire RFIs and Submittals API
  slug: fieldwire-rfis-submittals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-rfis-submittals-api-openapi.yml
- filename: fieldwire-webhooks-api-openapi.yml
  format: yaml
  label: Fieldwire Webhooks API
  slug: fieldwire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/openapi/fieldwire-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fieldwire.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.fieldwire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:39:36 2026 GMT
  host: developers.fieldwire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: client-api.super.fieldwire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fieldwire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fieldwire, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fieldwire
provider_slug: fieldwire
slug: fieldwire-domain-security
source_filename: fieldwire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fieldwire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n- host: developers.fieldwire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:39:36 2026 GMT\n  hsts: null\n- host: client-api.super.fieldwire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fieldwire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldwire/refs/heads/main/security/fieldwire-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Construction Technology
- ConTech
- Field Management
- Punch List
- Plans
- Drawings
- BIM
- Forms
- Inspections
- Project Management
- Hilti
---
