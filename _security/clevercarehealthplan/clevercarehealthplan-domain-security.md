---
api_specs:
- filename: clevercarehealthplan-drug-formulary-api-openapi.yml
  format: yaml
  label: Clever Care Health Plan Drug Formulary API
  slug: clevercarehealthplan-drug-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/openapi/clevercarehealthplan-drug-formulary-api-openapi.yml
- filename: clevercarehealthplan-patient-access-api-openapi.yml
  format: yaml
  label: Clever Care Health Plan Patient Access API
  slug: clevercarehealthplan-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/openapi/clevercarehealthplan-patient-access-api-openapi.yml
- filename: clevercarehealthplan-provider-directory-api-openapi.yml
  format: yaml
  label: Clever Care Health Plan Provider Directory API
  slug: clevercarehealthplan-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/openapi/clevercarehealthplan-provider-directory-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clevercarehealthplan.com
  spf: true
hosts:
- cert_expires: Oct 16 10:18:09 2026 GMT
  host: clevercarehealthplan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clevercarehealthplan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clever Care Health Plan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clever Care Health Plan
provider_slug: clevercarehealthplan
slug: clevercarehealthplan-domain-security
source_filename: clevercarehealthplan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clevercarehealthplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 10:18:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clevercarehealthplan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/security/clevercarehealthplan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Insurance
- Medicare Advantage
- FHIR
- Interoperability
- Patient Access
- Provider Directory
- Drug Formulary
---
