---
api_specs:
- filename: advancedmd-fhir-single-api-openapi.json
  format: json
  label: AdvancedMD FHIR Single API (US Core 6.1.0)
  slug: advancedmd-fhir-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-fhir-single-api-openapi.json
- filename: advancedmd-fhir-bulk-api-openapi.json
  format: json
  label: AdvancedMD FHIR Bulk API
  slug: advancedmd-fhir-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-fhir-bulk-api-openapi.json
- filename: advancedmd-application-access-apis-swagger.json
  format: json
  label: AdvancedMD Application Access APIs (Legacy Patient APIs)
  slug: advancedmd-application-access-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-application-access-apis-swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: advancedmd.com
  spf: true
hosts:
- cert_expires: Sep 14 22:12:57 2026 GMT
  host: www.advancedmd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: developer.advancedmd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: fhir.advancedmd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: providerapi.advancedmd.com
  hsts: false
  https: true
  note: FHIR + Bulk API host. Probed manually 2026-07-27; the automated pass keys off apis.yml website/portal hosts only.
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: ptapi.advancedmd.com
  hsts: false
  https: true
  note: Application Access API host. Probed manually 2026-07-27.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Advancedmd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdvancedMD, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AdvancedMD
provider_slug: advancedmd
slug: advancedmd-domain-security
source_filename: advancedmd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.advancedmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:12:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.advancedmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\n- host: fhir.advancedmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: null\n- host: providerapi.advancedmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: false\n  note: FHIR + Bulk API host. Probed manually 2026-07-27; the automated pass keys off apis.yml website/portal hosts only.\n- host: ptapi.advancedmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: false\n  note: Application Access API host. Probed manually 2026-07-27.\ndomains:\n- domain: advancedmd.com\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/security/advancedmd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- EHR
- EMR
- Practice Management
- Medical Billing
- FHIR
- HL7
- SMART on FHIR
- US Core
- Interoperability
- Revenue Cycle Management
- Scheduling
---
