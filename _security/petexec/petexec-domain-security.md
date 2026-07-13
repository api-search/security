---
api_specs:
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Owners API
  slug: petexec-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Pets API
  slug: petexec-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Reservations API
  slug: petexec-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Calendar API
  slug: petexec-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Services API
  slug: petexec-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Vaccinations API
  slug: petexec-vaccinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Billing & Reports API
  slug: petexec-billing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
- filename: petexec-openapi.yml
  format: yaml
  label: PetExec Company & Account API
  slug: petexec-company-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/openapi/petexec-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: petexec.net
  spf: true
hosts:
- cert_expires: Sep 29 12:16:57 2026 GMT
  host: www.petexec.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 21:36:11 2026 GMT
  host: secure.petexec.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: beta.petexec.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Petexec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PetExec, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PetExec
provider_slug: petexec
slug: petexec-domain-security
source_filename: petexec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.petexec.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:16:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.petexec.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:36:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: beta.petexec.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: petexec.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petexec/refs/heads/main/security/petexec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pet Care
- Boarding
- Daycare
- Grooming
- Training
- Business Management
- Pet Business Software
---
