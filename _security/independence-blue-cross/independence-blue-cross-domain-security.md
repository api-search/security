---
api_specs:
- filename: independence-blue-cross-formulary-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Formulary API
  slug: independence-blue-cross-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-formulary-api-openapi.yml
- filename: independence-blue-cross-patient-access-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Patient Access API
  slug: independence-blue-cross-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-patient-access-api-openapi.yml
- filename: independence-blue-cross-provider-directory-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Provider Directory API
  slug: independence-blue-cross-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-provider-directory-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ibx.com
  spf: true
hosts:
- cert_expires: Sep 27 03:30:26 2026 GMT
  host: devportal.ibx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: www.ibx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  8 01:01:07 2026 GMT
  host: eapics.ibx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Independence Blue Cross Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Independence Blue Cross, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Independence Blue Cross
provider_slug: independence-blue-cross
slug: independence-blue-cross-domain-security
source_filename: independence-blue-cross-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devportal.ibx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:30:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ibx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eapics.ibx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:01:07 2026 GMT\n  hsts: null\ndomains:\n- domain: ibx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/security/independence-blue-cross-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Health Insurance
- Blue Cross Blue Shield
- Managed Care
- Medicare
- Medicare Advantage
- Medicaid
- CHIP
- Commercial
- Dental
- Vision
- Behavioral Health
- Pharmacy Benefits
- Interoperability
- FHIR
- SMART on FHIR
- CMS
- Patient Access
- Provider Directory
- Drug Formulary
- Transparency In Coverage
---
