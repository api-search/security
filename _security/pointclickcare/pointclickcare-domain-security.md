---
api_specs:
- filename: pointclickcare-assessments-api-openapi.yml
  format: yaml
  label: PointClickCare Assessments API
  slug: pointclickcare-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-assessments-api-openapi.yml
- filename: pointclickcare-diagnoses-api-openapi.yml
  format: yaml
  label: PointClickCare Diagnoses API
  slug: pointclickcare-diagnoses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-diagnoses-api-openapi.yml
- filename: pointclickcare-facilities-api-openapi.yml
  format: yaml
  label: PointClickCare Facilities API
  slug: pointclickcare-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-facilities-api-openapi.yml
- filename: pointclickcare-medications-api-openapi.yml
  format: yaml
  label: PointClickCare Medications API
  slug: pointclickcare-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-medications-api-openapi.yml
- filename: pointclickcare-patients-api-openapi.yml
  format: yaml
  label: PointClickCare Patients API
  slug: pointclickcare-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-patients-api-openapi.yml
- filename: pointclickcare-vitals-api-openapi.yml
  format: yaml
  label: PointClickCare Vitals API
  slug: pointclickcare-vitals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/openapi/pointclickcare-vitals-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pointclickcare.com
  spf: true
hosts:
- cert_expires: Sep  3 23:59:59 2026 GMT
  host: developer.pointclickcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 05:04:37 2026 GMT
  host: www.pointclickcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.pointclickcare.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pointclickcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PointClickCare, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PointClickCare
provider_slug: pointclickcare
slug: pointclickcare-domain-security
source_filename: pointclickcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.pointclickcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.pointclickcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:04:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pointclickcare.com\n  https: false\ndomains:\n- domain: pointclickcare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/security/pointclickcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Long-Term Care
- Post-Acute Care
- EHR
- FHIR
- Senior Care
- Interoperability
---
