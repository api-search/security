---
api_specs:
- filename: aetna-endpoint-api-openapi.yml
  format: yaml
  label: Aetna Endpoint API
  slug: aetna-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-endpoint-api-openapi.yml
- filename: aetna-location-api-openapi.yml
  format: yaml
  label: Aetna Location API
  slug: aetna-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-location-api-openapi.yml
- filename: aetna-organization-api-openapi.yml
  format: yaml
  label: Aetna Organization API
  slug: aetna-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-organization-api-openapi.yml
- filename: aetna-organizationaffiliation-api-openapi.yml
  format: yaml
  label: Aetna Organization Affiliation API
  slug: aetna-organizationaffiliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-organizationaffiliation-api-openapi.yml
- filename: aetna-practitioner-api-openapi.yml
  format: yaml
  label: Aetna Practitioner API
  slug: aetna-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-practitioner-api-openapi.yml
- filename: aetna-providerdirectorydata-api-openapi.yml
  format: yaml
  label: Aetna Providerdirectorydata API
  slug: aetna-providerdirectorydata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-providerdirectorydata-api-openapi.yml
- filename: aetna-patient-access-api-openapi.yml
  format: yaml
  label: Aetna Patient Access API
  slug: aetna-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-patient-access-api-openapi.yml
- filename: aetna-provider-directory-api-openapi.yml
  format: yaml
  label: Aetna Provider Directory API
  slug: aetna-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-provider-directory-api-openapi.yml
- filename: aetna-healthcare-service-api-openapi.yml
  format: yaml
  label: Aetna Healthcare Service API
  slug: aetna-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-healthcare-service-api-openapi.yml
- filename: aetna-insurance-plan-api-openapi.yml
  format: yaml
  label: Aetna Insurance Plan API
  slug: aetna-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-insurance-plan-api-openapi.yml
- filename: aetna-practitioner-role-api-openapi.yml
  format: yaml
  label: Aetna Practitioner Role API
  slug: aetna-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-practitioner-role-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aetna.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.aetna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: apif1.aetna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: vteapif1.aetna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aetna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aetna, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aetna
provider_slug: aetna
slug: aetna-domain-security
source_filename: aetna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aetna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\n- host: apif1.aetna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\n- host: vteapif1.aetna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aetna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/security/aetna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health Insurance
- Healthcare
- FHIR
- Patient Access
- Provider Directory
- Drug Formulary
- Prior Authorization
- CMS Interoperability
- SMART on FHIR
- CARIN Blue Button
- Da Vinci
- Payers
- Fortune 100
- CVS Health
---
