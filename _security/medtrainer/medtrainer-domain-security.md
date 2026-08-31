---
api_specs:
- filename: medtrainer-departments-api-openapi.yml
  format: yaml
  label: MedTrainer Departments API
  slug: medtrainer-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/openapi/medtrainer-departments-api-openapi.yml
- filename: medtrainer-divisions-api-openapi.yml
  format: yaml
  label: MedTrainer Divisions API
  slug: medtrainer-divisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/openapi/medtrainer-divisions-api-openapi.yml
- filename: medtrainer-locations-api-openapi.yml
  format: yaml
  label: MedTrainer Locations API
  slug: medtrainer-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/openapi/medtrainer-locations-api-openapi.yml
- filename: medtrainer-positions-api-openapi.yml
  format: yaml
  label: MedTrainer Positions API
  slug: medtrainer-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/openapi/medtrainer-positions-api-openapi.yml
- filename: medtrainer-practitioner-categories-api-openapi.yml
  format: yaml
  label: MedTrainer Practitioner Categories API
  slug: medtrainer-practitioner-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/openapi/medtrainer-practitioner-categories-api-openapi.yml
- filename: medtrainer-practitioners-api-openapi.yml
  format: yaml
  label: MedTrainer Practitioners API
  slug: medtrainer-practitioners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/openapi/medtrainer-practitioners-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medtrainer.com
  spf: true
hosts:
- cert_expires: Nov 23 09:09:29 2026 GMT
  host: medtrainer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 11:19:42 2027 GMT
  host: api.medtrainer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medtrainer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedTrainer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MedTrainer
provider_slug: medtrainer
slug: medtrainer-domain-security
source_filename: medtrainer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medtrainer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 09:09:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.medtrainer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 11:19:42 2027 GMT\n  hsts: null\ndomains:\n- domain: medtrainer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medtrainer/refs/heads/main/security/medtrainer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Compliance
- Credentialing
- Learning Management
- Provider Directory
- FHIR
- HL7
- Training
- Risk Management
- Software-as-a-Service
---
