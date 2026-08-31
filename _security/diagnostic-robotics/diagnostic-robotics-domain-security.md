---
api_specs:
- filename: diagnostic-robotics-api-auth-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics API Auth API
  slug: diagnostic-robotics-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-api-auth-api-openapi.yml
- filename: diagnostic-robotics-dataset-upload-api-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Dataset Upload API
  slug: diagnostic-robotics-dataset-upload-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-dataset-upload-api-api-openapi.yml
- filename: diagnostic-robotics-default-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Default API
  slug: diagnostic-robotics-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-default-api-openapi.yml
- filename: diagnostic-robotics-patient-profile-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Patient Profile API
  slug: diagnostic-robotics-patient-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-patient-profile-api-openapi.yml
- filename: diagnostic-robotics-patients-v2-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Patients v2 API
  slug: diagnostic-robotics-patients-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-patients-v2-api-openapi.yml
- filename: diagnostic-robotics-questions-v2-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Questions v2 API
  slug: diagnostic-robotics-questions-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-questions-v2-api-openapi.yml
- filename: diagnostic-robotics-risk-adjustment-profile-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Risk Adjustment Profile API
  slug: diagnostic-robotics-risk-adjustment-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-risk-adjustment-profile-api-openapi.yml
- filename: diagnostic-robotics-risk-list-api-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Risk List API
  slug: diagnostic-robotics-risk-list-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-risk-list-api-api-openapi.yml
- filename: diagnostic-robotics-risk-profile-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Risk Profile API
  slug: diagnostic-robotics-risk-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-risk-profile-api-openapi.yml
- filename: diagnostic-robotics-visits-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Visits API
  slug: diagnostic-robotics-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-visits-api-openapi.yml
- filename: diagnostic-robotics-visits-v2-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Visits v2 API
  slug: diagnostic-robotics-visits-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-visits-v2-api-openapi.yml
- filename: diagnostic-robotics-widgets-api-api-openapi.yml
  format: yaml
  label: Diagnostic Robotics Widgets API
  slug: diagnostic-robotics-widgets-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/openapi/diagnostic-robotics-widgets-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diagnosticrobotics.com
  spf: true
hosts:
- cert_expires: Sep 16 08:34:52 2026 GMT
  host: diagnosticrobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:28:26 2026 GMT
  host: docs.diagnosticrobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 20:44:38 2026 GMT
  host: sandbox.precision-population-health.diagnosticrobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diagnostic Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diagnostic Robotics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diagnostic Robotics
provider_slug: diagnostic-robotics
slug: diagnostic-robotics-domain-security
source_filename: diagnostic-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diagnosticrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:34:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.diagnosticrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:28:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.precision-population-health.diagnosticrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:44:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: diagnosticrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diagnostic-robotics/refs/heads/main/security/diagnostic-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- healthcare
- clinical-ai
- population-health
- risk-adjustment
- predictive-analytics
- triage
- fhir
- claims-data
- care-management
- payers
- medical-coding
---
