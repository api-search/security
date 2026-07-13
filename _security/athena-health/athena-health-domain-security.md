---
api_specs:
- filename: athenahealth-athenaone-rest-api-openapi.yml
  format: yaml
  label: athenahealth athenaOne REST API
  slug: athenahealth-athenaone-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-athenaone-rest-api-openapi.yml
- filename: athenahealth-fhir-r4-api-openapi.yml
  format: yaml
  label: athenahealth FHIR R4 API
  slug: athenahealth-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-r4-api-openapi.yml
- filename: athenahealth-fhir-subscriptions-api-openapi.yml
  format: yaml
  label: athenahealth FHIR Subscriptions API
  slug: athenahealth-fhir-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-subscriptions-api-openapi.yml
- filename: athenahealth-fhir-bulk-data-api-openapi.yml
  format: yaml
  label: athenahealth FHIR Bulk Data Access API
  slug: athenahealth-fhir-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-fhir-bulk-data-api-openapi.yml
- filename: athenahealth-cds-hooks-api-openapi.yml
  format: yaml
  label: athenahealth CDS Hooks API
  slug: athenahealth-cds-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/openapi/athenahealth-cds-hooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: athenahealth.com
  spf: true
hosts:
- cert_expires: Aug 17 17:23:46 2026 GMT
  host: www.athenahealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: mydata.athenahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: docs.athenahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Athena Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for athenahealth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: athenahealth
provider_slug: athena-health
slug: athena-health-domain-security
source_filename: athena-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.athenahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:23:46 2026 GMT\n  hsts: null\n- host: mydata.athenahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\n- host: docs.athenahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: athenahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athena-health/refs/heads/main/security/athena-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EHR
- Electronic Health Records
- Healthcare
- HL7
- FHIR
- Interoperability
- Practice Management
- Revenue Cycle Management
- USCDI
- Cures Act
- SMART on FHIR
- CDS Hooks
- Cloud EHR
---
