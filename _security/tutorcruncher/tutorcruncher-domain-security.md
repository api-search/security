---
api_specs:
- filename: tutorcruncher-agents-api-openapi.yml
  format: yaml
  label: TutorCruncher Agents API
  slug: tutorcruncher-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-agents-api-openapi.yml
- filename: tutorcruncher-appointments-api-openapi.yml
  format: yaml
  label: TutorCruncher Appointments API
  slug: tutorcruncher-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-appointments-api-openapi.yml
- filename: tutorcruncher-clients-api-openapi.yml
  format: yaml
  label: TutorCruncher Clients API
  slug: tutorcruncher-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-clients-api-openapi.yml
- filename: tutorcruncher-contractors-api-openapi.yml
  format: yaml
  label: TutorCruncher Contractors API
  slug: tutorcruncher-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-contractors-api-openapi.yml
- filename: tutorcruncher-invoices-api-openapi.yml
  format: yaml
  label: TutorCruncher Invoices API
  slug: tutorcruncher-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-invoices-api-openapi.yml
- filename: tutorcruncher-payments-api-openapi.yml
  format: yaml
  label: TutorCruncher Payments API
  slug: tutorcruncher-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-payments-api-openapi.yml
- filename: tutorcruncher-recipients-api-openapi.yml
  format: yaml
  label: TutorCruncher Recipients API
  slug: tutorcruncher-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-recipients-api-openapi.yml
- filename: tutorcruncher-reference-api-openapi.yml
  format: yaml
  label: TutorCruncher Reference API
  slug: tutorcruncher-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-reference-api-openapi.yml
- filename: tutorcruncher-services-api-openapi.yml
  format: yaml
  label: TutorCruncher Services API
  slug: tutorcruncher-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-services-api-openapi.yml
- filename: tutorcruncher-webhooks-api-openapi.yml
  format: yaml
  label: TutorCruncher Webhooks API
  slug: tutorcruncher-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/openapi/tutorcruncher-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tutorcruncher.com
  spf: true
hosts:
- cert_expires: Aug 12 17:59:45 2026 GMT
  host: tutorcruncher.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 17:45:51 2026 GMT
  host: api.tutorcruncher.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 04:15:32 2026 GMT
  host: app.tutorcruncher.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tutorcruncher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TutorCruncher, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TutorCruncher
provider_slug: tutorcruncher
slug: tutorcruncher-domain-security
source_filename: tutorcruncher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tutorcruncher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:59:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tutorcruncher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:45:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.tutorcruncher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:15:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tutorcruncher.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tutorcruncher/refs/heads/main/security/tutorcruncher-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Tutoring
- Education
- Business Management
- Scheduling
- Invoicing
- Payments
- EdTech
---
