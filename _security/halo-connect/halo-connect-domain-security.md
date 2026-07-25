---
api_specs:
- filename: halo-connect-integrator-openapi.json
  format: json
  label: Halo Cloud API for Integrators
  slug: halo-cloud-integrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-integrator-openapi.json
- filename: halo-connect-desktop-openapi.json
  format: json
  label: Halo Cloud API for Desktop Applications
  slug: halo-cloud-desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-desktop-openapi.json
- filename: halo-connect-integrator-openapi.json
  format: json
  label: Halo Cloud FHIR API
  slug: halo-cloud-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/openapi/halo-connect-integrator-openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haloconnect.io
  spf: true
hosts:
- cert_expires: Sep  3 00:00:06 2026 GMT
  host: haloconnect.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.haloconnect.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 23:20:37 2026 GMT
  host: api.haloconnect.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Halo Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Halo Connect, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Halo Connect
provider_slug: halo-connect
slug: halo-connect-domain-security
source_filename: halo-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haloconnect.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:00:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.haloconnect.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.haloconnect.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:20:37 2026 GMT\n  hsts: null\ndomains:\n- domain: haloconnect.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halo-connect/refs/heads/main/security/halo-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Australia
- FHIR
- HL7
- Interoperability
- EHR
- Practice Management
- Primary Care
- AU Base
- Health Data
---
