---
api_specs:
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Scheduling & Appointments API
  slug: luma-health-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Patients API
  slug: luma-health-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Providers & Facilities API
  slug: luma-health-providers-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Messaging & Engagement API
  slug: luma-health-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Broadcast & Campaigns API
  slug: luma-health-broadcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Intake & Forms API
  slug: luma-health-intake-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Billing & Payments API
  slug: luma-health-billing-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Eligibility & Insurance API
  slug: luma-health-eligibility-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Referrals API
  slug: luma-health-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Feedback & Reputation API
  slug: luma-health-feedback-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Conversational AI Assistant API
  slug: luma-health-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Reporting & Audits API
  slug: luma-health-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
- filename: luma-health-openapi.yaml
  format: yaml
  label: Luma Health Authentication API
  slug: luma-health-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/openapi/luma-health-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lumahealth.io
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.lumahealth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: apidocs.lumahealth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.lumahealth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luma Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luma Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Luma Health
provider_slug: luma-health
slug: luma-health-domain-security
source_filename: luma-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lumahealth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.lumahealth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lumahealth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lumahealth.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luma-health/refs/heads/main/security/luma-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United States
- Patient Engagement
- Scheduling
- Referrals
- Intake
- Messaging
- Eligibility
- EHR
- Interoperability
- Clinical AI
- Reputation Management
- Patient Feedback
---
