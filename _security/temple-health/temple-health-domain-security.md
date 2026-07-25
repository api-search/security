---
api_specs:
- filename: temple-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Temple Health Allergy Intolerance API
  slug: temple-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-allergy-intolerance-api-openapi.yml
- filename: temple-health-bulk-data-api-openapi.yml
  format: yaml
  label: Temple Health Bulk Data API
  slug: temple-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-bulk-data-api-openapi.yml
- filename: temple-health-condition-api-openapi.yml
  format: yaml
  label: Temple Health Condition API
  slug: temple-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-condition-api-openapi.yml
- filename: temple-health-document-reference-api-openapi.yml
  format: yaml
  label: Temple Health Document Reference API
  slug: temple-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-document-reference-api-openapi.yml
- filename: temple-health-encounter-api-openapi.yml
  format: yaml
  label: Temple Health Encounter API
  slug: temple-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-encounter-api-openapi.yml
- filename: temple-health-medication-request-api-openapi.yml
  format: yaml
  label: Temple Health Medication Request API
  slug: temple-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-medication-request-api-openapi.yml
- filename: temple-health-metadata-api-openapi.yml
  format: yaml
  label: Temple Health Metadata API
  slug: temple-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-metadata-api-openapi.yml
- filename: temple-health-observation-api-openapi.yml
  format: yaml
  label: Temple Health Observation API
  slug: temple-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-observation-api-openapi.yml
- filename: temple-health-patient-api-openapi.yml
  format: yaml
  label: Temple Health Patient API
  slug: temple-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-patient-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: templehealth.org
  spf: true
hosts:
- cert_expires: Sep 14 01:30:17 2026 GMT
  host: www.templehealth.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: epicaccess.templehealth.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: my.templehealth.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Temple Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temple Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Temple Health
provider_slug: temple-health
slug: temple-health-domain-security
source_filename: temple-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.templehealth.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:30:17 2026 GMT\n  hsts: false\n- host: epicaccess.templehealth.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\n- host: my.templehealth.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: templehealth.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/security/temple-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Academic Medical Center
- CMS Interoperability
- Cures Act
- DSTU2
- Epic
- FHIR
- Fox Chase Cancer Center
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Price Transparency
- R4
- SMART on FHIR
- Temple University
- US Core
- USCDI
---
