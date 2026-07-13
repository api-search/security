---
api_specs:
- filename: cigna-patient-access-api-openapi.yml
  format: yaml
  label: Cigna Patient Access API
  slug: patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-patient-access-api-openapi.yml
- filename: cigna-provider-directory-api-openapi.yml
  format: yaml
  label: Cigna Provider Directory API
  slug: provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-provider-directory-api-openapi.yml
- filename: cigna-drug-formulary-api-openapi.yml
  format: yaml
  label: Cigna Drug Formulary API
  slug: drug-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-drug-formulary-api-openapi.yml
- filename: cigna-provider-access-api-openapi.yml
  format: yaml
  label: Cigna Provider Access API
  slug: provider-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-provider-access-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cigna.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.cigna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: developer.cigna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: fhir.cigna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cigna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cigna, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cigna
provider_slug: cigna
slug: cigna-domain-security
source_filename: cigna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cigna.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.cigna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fhir.cigna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cigna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/security/cigna-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- CMS Interoperability
- Da Vinci
- Drug Formulary
- FHIR
- Health Insurance
- Healthcare
- Patient Access
- Provider Directory
- SMART on FHIR
- Fortune 100
---
