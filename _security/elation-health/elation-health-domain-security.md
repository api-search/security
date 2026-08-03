---
api_specs:
- filename: elation-api-authentication.json
  format: json
  label: Elation OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-api-authentication.json
- filename: elation-patient-profile-api.json
  format: json
  label: Elation Patient Profile API
  slug: patient-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-patient-profile-api.json
- filename: elation-visit-notes-api.json
  format: json
  label: Elation Visit Notes API
  slug: visit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-visit-notes-api.json
- filename: elation-patient-document-api.json
  format: json
  label: Elation Patient Document API
  slug: patient-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-patient-document-api.json
- filename: elation-orders-api.json
  format: json
  label: Elation Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-orders-api.json
- filename: elation-scheduling-api.json
  format: json
  label: Elation Scheduling API
  slug: scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-scheduling-api.json
- filename: elation-billing-api.json
  format: json
  label: Elation Billing API
  slug: billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-billing-api.json
- filename: elation-insurance-api.json
  format: json
  label: Elation Insurance API
  slug: insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-insurance-api.json
- filename: elation-premium-patient-insurance-api.json
  format: json
  label: Elation Patient Insurance API (Premium) & Eligibility
  slug: patient-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-premium-patient-insurance-api.json
- filename: elation-practice-api.json
  format: json
  label: Elation Practice API
  slug: practice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-practice-api.json
- filename: elation-user-management-api.json
  format: json
  label: Elation User Management API
  slug: user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-user-management-api.json
- filename: elation-messaging-api.json
  format: json
  label: Elation Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-messaging-api.json
- filename: elation-event-subscription-api.json
  format: json
  label: Elation Event Subscription API
  slug: event-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-event-subscription-api.json
- filename: elation-reference-data-api.json
  format: json
  label: Elation Reference Data API
  slug: reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-reference-data-api.json
- filename: elation-care-gaps-api-1.json
  format: json
  label: Elation Care Gaps API
  slug: care-gaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-care-gaps-api-1.json
- filename: elation-elation-import-api.json
  format: json
  label: Elation Import API
  slug: import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-elation-import-api.json
- filename: elation-api-settings.json
  format: json
  label: Elation Health API Settings
  slug: elation-api-settings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/openapi/elation-api-settings.json
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
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: api.app.elationemr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elation Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elation Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Elation Health
provider_slug: elation-health
slug: elation-health-domain-security
source_filename: elation-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elationhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.elationhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:56:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.app.elationemr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: elationhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: elationemr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation-health/refs/heads/main/security/elation-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Primary Care
- Value-Based Care
- Eligibility
- Clinical Data
- Scheduling
- e-Prescribing
- Digital Health
---
