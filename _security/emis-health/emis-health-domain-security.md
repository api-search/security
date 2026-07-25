---
api_specs:
- filename: emis-health-partner-api-openapi.json
  format: json
  label: EMIS Partner API (PAPI)
  slug: emis-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emis-health/refs/heads/main/openapi/emis-health-partner-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: emishealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emis-x.uk
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: www.emishealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 12:23:57 2026 GMT
  host: docs.partner.emis-x.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.platform.emis-x.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emis Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EMIS Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EMIS Health
provider_slug: emis-health
slug: emis-health-domain-security
source_filename: emis-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.partner.emis-x.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.platform.emis-x.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: emishealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: emis-x.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emis-health/refs/heads/main/security/emis-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United Kingdom
- EHR
- EMR
- Interoperability
- HL7
- FHIR
- Primary Care
- NHS
- Clinical Data
- Electronic Patient Record
---
