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
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: templehealth.org
  spf: true
hosts:
- cert_expires: Nov 12 00:46:51 2026 GMT
  host: www.templehealth.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: epicaccess.templehealth.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Temple Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temple Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Temple Health
provider_slug: temple-health
slug: temple-health-domain-security
source_filename: temple-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.templehealth.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 00:46:51 2026 GMT\n  hsts: false\n- host: epicaccess.templehealth.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: templehealth.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnotes:\n- 'HSTS discrepancy, observed 2026-08-15: the mechanical probe records hsts:false for epicaccess.templehealth.org\n  because the origin-root 404 page carries no HSTS header. The FHIR API paths on that same host DO return\n  \"strict-transport-security: max-age=31536000; includeSubDomains\" on both 200 and 401 responses. The\n  API surface is HSTS-protected; the host root is not.'\n- 'my.templehealth.org\
  \ (the myTempleHealth/MyChart portal) is not in the probed host list because it is\n  carried as a PatientPortal property rather than a baseURL. Probed separately 2026-08-15: HTTPS, TLSv1.2,\n  HSTS present with max-age 31536000.'\n- No security.txt on any Temple Health host, so no RFC 9116 contact exists for reporting a finding against\n  these hosts. See well-known/temple-health-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/security/temple-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
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
- Authentication
- Patient Access
- Price Transparency
- R4
- SMART on FHIR
- Temple University
- US Core
- USCDI
---
