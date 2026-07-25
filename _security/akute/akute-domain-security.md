---
api_specs:
- filename: akute-appointments-api-openapi.yml
  format: yaml
  label: Akute Health Appointments API
  slug: akute-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-appointments-api-openapi.yml
- filename: akute-documents-api-openapi.yml
  format: yaml
  label: Akute Health Documents API
  slug: akute-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-documents-api-openapi.yml
- filename: akute-encounters-api-openapi.yml
  format: yaml
  label: Akute Health Encounters API
  slug: akute-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-encounters-api-openapi.yml
- filename: akute-labs-api-openapi.yml
  format: yaml
  label: Akute Health Labs API
  slug: akute-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-labs-api-openapi.yml
- filename: akute-medications-api-openapi.yml
  format: yaml
  label: Akute Health Medications API
  slug: akute-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-medications-api-openapi.yml
- filename: akute-patients-api-openapi.yml
  format: yaml
  label: Akute Health Patients API
  slug: akute-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-patients-api-openapi.yml
- filename: akute-tasks-api-openapi.yml
  format: yaml
  label: Akute Health Tasks API
  slug: akute-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-tasks-api-openapi.yml
- filename: akute-webhooks-api-openapi.yml
  format: yaml
  label: Akute Health Webhooks API
  slug: akute-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/openapi/akute-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: akutehealth.com
  spf: true
hosts:
- cert_expires: Oct  6 08:54:58 2026 GMT
  host: www.akutehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 20:10:23 2026 GMT
  host: developer.akutehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: api.akutehealth.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Akute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akute Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Akute Health
provider_slug: akute
slug: akute-domain-security
source_filename: akute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akutehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:54:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.akutehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:10:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.akutehealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: akutehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akute/refs/heads/main/security/akute-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- EHR
- EMR
- FHIR
- Digital Health
- Telehealth
---
