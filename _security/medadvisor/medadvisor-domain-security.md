---
api_specs:
- filename: medadvisor-3rd-party-integration-api-openapi.yml
  format: yaml
  label: MedAdvisor 3rd-Party Integration API
  slug: medadvisor-3rd-party-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-3rd-party-integration-api-openapi.yml
- filename: medadvisor-account-api-openapi.yml
  format: yaml
  label: MedAdvisor Account API
  slug: medadvisor-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-account-api-openapi.yml
- filename: medadvisor-booking-api-openapi.yml
  format: yaml
  label: MedAdvisor Booking API
  slug: medadvisor-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-booking-api-openapi.yml
- filename: medadvisor-bookingservice-api-openapi.yml
  format: yaml
  label: MedAdvisor Booking Service API
  slug: medadvisor-bookingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-bookingservice-api-openapi.yml
- filename: medadvisor-calendarsetting-api-openapi.yml
  format: yaml
  label: MedAdvisor Calendar Setting API
  slug: medadvisor-calendarsetting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-calendarsetting-api-openapi.yml
- filename: medadvisor-clinic-api-openapi.yml
  format: yaml
  label: MedAdvisor Clinic API
  slug: medadvisor-clinic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-clinic-api-openapi.yml
- filename: medadvisor-communication-api-openapi.yml
  format: yaml
  label: MedAdvisor Communication API
  slug: medadvisor-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-communication-api-openapi.yml
- filename: medadvisor-config-api-openapi.yml
  format: yaml
  label: MedAdvisor Config API
  slug: medadvisor-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-config-api-openapi.yml
- filename: medadvisor-headoffice-api-openapi.yml
  format: yaml
  label: MedAdvisor Head Office API
  slug: medadvisor-headoffice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-headoffice-api-openapi.yml
- filename: medadvisor-inbox-api-openapi.yml
  format: yaml
  label: MedAdvisor Inbox API
  slug: medadvisor-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-inbox-api-openapi.yml
- filename: medadvisor-logging-api-openapi.yml
  format: yaml
  label: MedAdvisor Logging API
  slug: medadvisor-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-logging-api-openapi.yml
- filename: medadvisor-pharmacist-api-openapi.yml
  format: yaml
  label: MedAdvisor Pharmacist API
  slug: medadvisor-pharmacist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacist-api-openapi.yml
- filename: medadvisor-pharmacy-api-openapi.yml
  format: yaml
  label: MedAdvisor Pharmacy API
  slug: medadvisor-pharmacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-api-openapi.yml
- filename: medadvisor-refillorder-api-openapi.yml
  format: yaml
  label: MedAdvisor Refill Order API
  slug: medadvisor-refillorder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-refillorder-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medadvisor.com.au
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.medadvisor.com.au
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: pharmacy-unified.api.medadvisor.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Medadvisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedAdvisor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MedAdvisor
provider_slug: medadvisor
slug: medadvisor-domain-security
source_filename: medadvisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medadvisor.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\n- host: pharmacy-unified.api.medadvisor.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: medadvisor.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/security/medadvisor-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Healthcare
- Australia
- Pharmacy
- Medication Management
- Medication Adherence
- e-Prescribing
- eScript
- Patient Engagement
- Appointment Booking
- Digital Health
- Healthcare API
---
