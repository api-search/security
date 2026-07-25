---
api_specs:
- filename: nhsd-developers-portal.postman_collection.json
  format: json
  label: NHSD FHIR API
  slug: nhsd-fhir-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/healthdirect/refs/heads/main/collections/nhsd-developers-portal.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: healthdirect.gov.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: healthdirect.org.au
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: about.healthdirect.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.fhir.int.nhsd.healthdirect.org.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: build.fhir.nhsd.healthdirect.org.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthdirect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Healthdirect Australia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Healthdirect Australia
provider_slug: healthdirect
slug: healthdirect-domain-security
source_filename: healthdirect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: about.healthdirect.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\n- host: api.fhir.int.nhsd.healthdirect.org.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\n- host: build.fhir.nhsd.healthdirect.org.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: healthdirect.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: healthdirect.org.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthdirect/refs/heads/main/security/healthdirect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Australia
- FHIR
- HL7
- Interoperability
- Provider Directory
- National Health System
- Health Services Directory
- Telehealth
- Digital Health
- Appointments
---
