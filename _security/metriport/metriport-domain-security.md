---
api_specs:
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Medical Patients API
  slug: medical-patients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Medical Facilities API
  slug: medical-facilities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Medical Document Query API
  slug: medical-document-query
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Medical Consolidated FHIR API
  slug: medical-consolidated-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Devices Users API
  slug: devices-users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Devices Biometrics API
  slug: devices-biometrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
- filename: metriport-openapi.yml
  format: yaml
  label: Metriport Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metriport.com
  spf: true
hosts:
- cert_expires: Aug 20 03:59:08 2026 GMT
  host: www.metriport.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 00:37:00 2026 GMT
  host: docs.metriport.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.metriport.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metriport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metriport, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metriport
provider_slug: metriport
slug: metriport-domain-security
source_filename: metriport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metriport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 03:59:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.metriport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 00:37:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.metriport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: metriport.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/security/metriport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Records
- FHIR
- Health Data
- Wearables
- Open Source
---
