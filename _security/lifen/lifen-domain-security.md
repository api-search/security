---
api_specs:
- filename: lifen-communicationrequest-api-openapi.yml
  format: yaml
  label: Lifen CommunicationRequest API
  slug: lifen-communicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-communicationrequest-api-openapi.yml
- filename: lifen-coverage-api-openapi.yml
  format: yaml
  label: Lifen Coverage API
  slug: lifen-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-coverage-api-openapi.yml
- filename: lifen-encounter-api-openapi.yml
  format: yaml
  label: Lifen Encounter API
  slug: lifen-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-encounter-api-openapi.yml
- filename: lifen-organization-api-openapi.yml
  format: yaml
  label: Lifen Organization API
  slug: lifen-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-organization-api-openapi.yml
- filename: lifen-patient-api-openapi.yml
  format: yaml
  label: Lifen Patient API
  slug: lifen-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-patient-api-openapi.yml
- filename: lifen-practitioner-api-openapi.yml
  format: yaml
  label: Lifen Practitioner API
  slug: lifen-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-practitioner-api-openapi.yml
- filename: lifen-token-api-openapi.yml
  format: yaml
  label: Lifen Token API
  slug: lifen-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/openapi/lifen-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lifen.fr
  spf: true
hosts:
- cert_expires: Sep 21 21:48:23 2026 GMT
  host: www.lifen.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 08:03:39 2026 GMT
  host: developer.lifen.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.lifen.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lifen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lifen, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lifen
provider_slug: lifen
slug: lifen-domain-security
source_filename: lifen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lifen.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:48:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lifen.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:03:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lifen.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lifen.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifen/refs/heads/main/security/lifen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- FHIR
- Interoperability
- Health Data
- Electronic Health Records
- Medical Documents
- Secure Messaging
- France
- HL7
---
