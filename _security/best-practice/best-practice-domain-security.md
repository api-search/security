---
api_specs:
- filename: haloconnect-integrator-openapi.json
  format: json
  label: Halo Cloud API for Integrators
  slug: halo-cloud-integrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/haloconnect-integrator-openapi.json
- filename: haloconnect-desktop-openapi.json
  format: json
  label: Halo Cloud API for Desktop Applications
  slug: halo-cloud-desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/haloconnect-desktop-openapi.json
- filename: haloconnect-integrator-openapi.json
  format: json
  label: FHIR API for Bp Premier
  slug: fhir-api-bp-premier
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/openapi/haloconnect-integrator-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bpsoftware.net
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haloconnect.io
  spf: true
hosts:
- cert_expires: Oct  6 07:43:02 2026 GMT
  host: bpsoftware.net
  hsts: false
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
name: Best Practice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Best Practice Software, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Best Practice Software
provider_slug: best-practice
slug: best-practice-domain-security
source_filename: best-practice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bpsoftware.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 07:43:02 2026 GMT\n  hsts: false\n- host: docs.haloconnect.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.haloconnect.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:20:37 2026 GMT\n  hsts: null\ndomains:\n- domain: bpsoftware.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: haloconnect.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/best-practice/refs/heads/main/security/best-practice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Australia
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- AU Base
- Practice Management
- General Practice
- Appointments
- Scheduling
---
