---
api_specs:
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - 3rd-Party Integration
  slug: pharmacy-unified-third-party-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Booking Service
  slug: pharmacy-unified-booking-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Refill Order
  slug: pharmacy-unified-refill-order
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Inbox
  slug: pharmacy-unified-inbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Communication
  slug: pharmacy-unified-communication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Head Office
  slug: pharmacy-unified-head-office
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
- filename: medadvisor-pharmacy-unified-openapi.json
  format: json
  label: Pharmacy Unified API - Pharmacy
  slug: pharmacy-unified-pharmacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medadvisor/refs/heads/main/openapi/medadvisor-pharmacy-unified-openapi.json
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
