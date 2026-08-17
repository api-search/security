---
api_specs:
- filename: tebra-documents-api-openapi.yml
  format: yaml
  label: Tebra Documents API
  slug: tebra-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-documents-api-openapi.yml
- filename: tebra-clinical-api-openapi.yml
  format: yaml
  label: Tebra Clinical API
  slug: tebra-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-clinical-api-openapi.yml
- filename: tebra-documents-api-openapi.yml
  format: yaml
  label: Tebra Documents API
  slug: tebra-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-documents-api-openapi.yml
- filename: tebra-patient-api-openapi.yml
  format: yaml
  label: Tebra Patient API
  slug: tebra-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-patient-api-openapi.yml
- filename: tebra-fhir-api-openapi.yml
  format: yaml
  label: Tebra FHIR API
  slug: tebra-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/openapi/tebra-fhir-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:netops-team@kareo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tebra.com
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:netops-team@kareo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kareo.com
  spf: true
hosts:
- cert_expires: Oct 29 01:46:25 2026 GMT
  host: www.tebra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: helpme.tebra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: webservice.kareo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 07:51:50 2026 GMT
  host: fhir.prd.cloud.tebra.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  note: Manually probed (openssl s_client + curl, 2026-08-14); not covered by the automated 3-host cap. Live SMART on FHIR host (tebra:tebra-fhir-api).
  tls_version: TLSv1.3
- dns_status: NXDOMAIN
  host: api.tebra.com
  https: null
  note: Host documented as the Clinical Data API base in Tebra's own Oct 2023 "General API Documentation" PDF and in this repo's openapi/ servers[], but fails to resolve on public DNS resolvers (system, 8.8.8.8, 1.1.1.1) as of 2026-08-14. See lifecycle/tebra-lifecycle.yml.
kind: domain-security
layout: security
method: probed
name: Tebra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tebra, probed live across 5 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tebra
provider_slug: tebra
slug: tebra-domain-security
source_filename: tebra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 01:46:25 2026 GMT\n  hsts: false\n- host: helpme.tebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webservice.kareo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\n- host: fhir.prd.cloud.tebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 07:51:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  note: >-\n    Manually probed (openssl s_client + curl, 2026-08-14); not covered by the\n    automated 3-host cap. Live SMART on FHIR host (tebra:tebra-fhir-api).\n- host: api.tebra.com\n  https: null\n  dns_status: NXDOMAIN\n  note: >-\n    Host documented as the Clinical Data API base in Tebra's own Oct 2023\n    \"General API\
  \ Documentation\" PDF and in this repo's openapi/ servers[], but\n    fails to resolve on public DNS resolvers (system, 8.8.8.8, 1.1.1.1) as of\n    2026-08-14. See lifecycle/tebra-lifecycle.yml.\ndomains:\n- domain: tebra.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:netops-team@kareo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kareo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:netops-team@kareo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tebra/refs/heads/main/security/tebra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Practice Management
- EHR
- Medical Billing
- Patient Engagement
- Kareo
- PatientPop
---
