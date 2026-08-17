---
api_specs:
- filename: cerner-millennium-fhir-r4-openapi.yml
  format: yaml
  label: Oracle Health Millennium Platform FHIR R4 API
  slug: oracle-health-millennium-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-millennium-fhir-r4-openapi.yml
- filename: cerner-millennium-bulk-data-openapi.yml
  format: yaml
  label: Oracle Health Millennium Bulk FHIR API
  slug: oracle-health-bulk-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-millennium-bulk-data-openapi.yml
- filename: cerner-capability-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Capability API
  slug: cerner-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-capability-api-openapi.yml
- filename: cerner-condition-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Condition API
  slug: cerner-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-condition-api-openapi.yml
- filename: cerner-definitions-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Definitions API
  slug: cerner-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-definitions-api-openapi.yml
- filename: cerner-encounter-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Encounter API
  slug: cerner-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-encounter-api-openapi.yml
- filename: cerner-generic-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Generic API
  slug: cerner-generic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-generic-api-openapi.yml
- filename: cerner-patient-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Patient API
  slug: cerner-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-patient-api-openapi.yml
- filename: cerner-procedure-api-openapi.yml
  format: yaml
  label: Cerner (Oracle Health) Procedure API
  slug: cerner-procedure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-procedure-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cerner.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.cerner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: fhir.cerner.com
  hsts: false
  https: true
  note: 301s to docs.oracle.com — documentation host only, no longer serves the API.
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: fhir-ehr.cerner.com
  hsts: false
  https: true
  role: production FHIR R4 service root (provider persona)
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: fhir-ehr-code.cerner.com
  hsts: false
  https: true
  role: secure sandbox FHIR R4 service root
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: fhir-open.cerner.com
  hsts: false
  https: true
  role: open, unauthenticated, read-only FHIR R4 service root
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: fhir-myrecord.cerner.com
  hsts: false
  https: true
  role: patient-access FHIR R4 service root
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: authorization.cerner.com
  hsts: false
  https: true
  role: SMART on FHIR authorization server (token, authorize, revoke, introspect, JWKS)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Health (Cerner), probed live across 8 host(s) and 2 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Health (Cerner)
provider_slug: cerner
slug: cerner-domain-security
source_filename: cerner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cerner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: fhir.cerner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\n  note: 301s to docs.oracle.com — documentation host only, no longer serves the API.\n# The five hosts below are the LIVE API and authorization hosts. They are not reachable from the\n# apis.yml Website/Portal fields the automated probe reads, so they were probed by hand on 2026-08-14\n# (openssl s_client for TLS and cert expiry, curl -I for HSTS).\n- host: fhir-ehr.cerner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n  role: production\
  \ FHIR R4 service root (provider persona)\n- host: fhir-ehr-code.cerner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n  role: secure sandbox FHIR R4 service root\n- host: fhir-open.cerner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n  role: open, unauthenticated, read-only FHIR R4 service root\n- host: fhir-myrecord.cerner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n  role: patient-access FHIR R4 service root\n- host: authorization.cerner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n  role: SMART on FHIR authorization server (token, authorize, revoke, introspect, JWKS)\nfindings:\n- >-\n  No HSTS on any of the five live API/authorization hosts, including the OAuth 2.0 authorization server\n  that issues tokens carrying PHI scopes. Only the marketing host www.cerner.com\
  \ sets\n  Strict-Transport-Security. This is the most notable gap in this profile.\n- >-\n  cerner.com publishes no CAA record, so no certificate authority is pinned for the domain that hosts\n  every live API endpoint. oracle.com does pin three (digicert, pki.goog, letsencrypt).\n- No DNSSEC on either registrable domain.\n- SPF and DMARC are present on both domains with DMARC policy p=reject.\ndomains:\n- domain: cerner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/security/cerner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bulk FHIR
- CapabilityStatement
- CareAware
- Cerner Millennium
- Clinical Data
- Code Console
- EHR
- Electronic Health Records
- FHIR
- Fortune 1000
- HL7
- HL7 v2
- Healthcare
- Interoperability
- Millennium Platform
- Multi-Tenant
- OAuth 2.0
- Oracle
- Oracle Health
- Patient Access
- Provider Directory
- SMART Backend Services
- SMART on FHIR
- US Core
---
