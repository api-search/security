---
api_specs:
- filename: elation-allergies-api-openapi.yml
  format: yaml
  label: Elation Health Allergies API
  slug: elation-allergies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-allergies-api-openapi.yml
- filename: elation-appointments-api-openapi.yml
  format: yaml
  label: Elation Health Appointments API
  slug: elation-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-appointments-api-openapi.yml
- filename: elation-authentication-api-openapi.yml
  format: yaml
  label: Elation Health Authentication API
  slug: elation-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-authentication-api-openapi.yml
- filename: elation-billing-api-openapi.yml
  format: yaml
  label: Elation Health Billing API
  slug: elation-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-billing-api-openapi.yml
- filename: elation-insurance-api-openapi.yml
  format: yaml
  label: Elation Health Insurance API
  slug: elation-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-insurance-api-openapi.yml
- filename: elation-lab-orders-api-openapi.yml
  format: yaml
  label: Elation Health Lab Orders API
  slug: elation-lab-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-lab-orders-api-openapi.yml
- filename: elation-medications-api-openapi.yml
  format: yaml
  label: Elation Health Medications API
  slug: elation-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-medications-api-openapi.yml
- filename: elation-messaging-api-openapi.yml
  format: yaml
  label: Elation Health Messaging API
  slug: elation-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-messaging-api-openapi.yml
- filename: elation-patients-api-openapi.yml
  format: yaml
  label: Elation Health Patients API
  slug: elation-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-patients-api-openapi.yml
- filename: elation-physicians-api-openapi.yml
  format: yaml
  label: Elation Health Physicians API
  slug: elation-physicians-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-physicians-api-openapi.yml
- filename: elation-practices-api-openapi.yml
  format: yaml
  label: Elation Health Practices API
  slug: elation-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-practices-api-openapi.yml
- filename: elation-problems-api-openapi.yml
  format: yaml
  label: Elation Health Problems API
  slug: elation-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-problems-api-openapi.yml
- filename: elation-visit-notes-api-openapi.yml
  format: yaml
  label: Elation Health Visit Notes API
  slug: elation-visit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/openapi/elation-visit-notes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elationhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elationemr.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.elationhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:56:34 2026 GMT
  host: docs.elationhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: app.elationemr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elation Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Elation Health
provider_slug: elation
slug: elation-domain-security
source_filename: elation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elationhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.elationhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:56:34 2026 GMT\n  hsts: null\n- host: app.elationemr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: elationhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: elationemr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/security/elation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EHR
- Electronic Health Records
- Primary Care
- Healthcare
- FHIR
- Clinical
- Patients
- Prescriptions
- Messaging
---
