---
api_specs:
- filename: metriport-consolidated-api-openapi.yml
  format: yaml
  label: Metriport Consolidated API
  slug: metriport-consolidated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-consolidated-api-openapi.yml
- filename: metriport-devices-data-api-openapi.yml
  format: yaml
  label: Metriport Devices Data API
  slug: metriport-devices-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-devices-data-api-openapi.yml
- filename: metriport-document-api-openapi.yml
  format: yaml
  label: Metriport Document API
  slug: metriport-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-document-api-openapi.yml
- filename: metriport-facility-api-openapi.yml
  format: yaml
  label: Metriport Facility API
  slug: metriport-facility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-facility-api-openapi.yml
- filename: metriport-patient-api-openapi.yml
  format: yaml
  label: Metriport Patient API
  slug: metriport-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-patient-api-openapi.yml
- filename: metriport-settings-api-openapi.yml
  format: yaml
  label: Metriport Settings API
  slug: metriport-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-settings-api-openapi.yml
- filename: metriport-user-api-openapi.yml
  format: yaml
  label: Metriport User API
  slug: metriport-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metriport.com
  spf: true
hosts:
- cert_expires: Oct 18 07:46:53 2026 GMT
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
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metriport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 07:46:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.metriport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 00:37:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.metriport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: metriport.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/security/metriport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Records
- FHIR
- Health Data
- Wearables
- Open-Source
---
