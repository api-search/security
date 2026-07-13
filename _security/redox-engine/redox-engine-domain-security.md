---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: redoxengine.com
  spf: true
hosts:
- cert_expires: Sep 25 20:13:48 2026 GMT
  host: www.redoxengine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: docs.redoxengine.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.redoxengine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redox Engine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Redox
provider_slug: redox-engine
slug: redox-engine-domain-security
source_filename: redox-engine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redoxengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.redoxengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.redoxengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: redoxengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redox-engine/refs/heads/main/security/redox-engine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bulk Data
- CDA
- Carequality
- CommonWell
- DICOM
- Data Model API
- Digital Health
- EHR
- EMPI
- Electronic Health Records
- FHIR
- HL7
- HL7v2
- Healthcare
- Healthcare Interoperability
- Integration Platform
- OAuth 2.0
- Patient Data
- Payers
- Platform API
- Providers
- R4
- SMART on FHIR
- TEFCA
- X12
---
