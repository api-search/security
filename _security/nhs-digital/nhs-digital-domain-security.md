---
api_specs:
- filename: booking-and-referral-fhir-api.yaml
  format: yaml
  label: Booking and Referral - FHIR API
  slug: booking-and-referral-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/booking-and-referral-fhir-api.yaml
- filename: nhs-app-api.yaml
  format: yaml
  label: NHS App API
  slug: nhs-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-app-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhs.uk
  spf: true
hosts:
- cert_expires: Sep 24 21:58:44 2026 GMT
  host: digital.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.service.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: sandbox.api.service.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nhs Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NHS Digital, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NHS Digital
provider_slug: nhs-digital
slug: nhs-digital-domain-security
source_filename: nhs-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digital.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:44 2026 GMT\n  hsts: null\n- host: api.service.nhs.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox.api.service.nhs.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nhs.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/security/nhs-digital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- NHS
- health
- FHIR
- UK
- patient demographics
- prescriptions
- referrals
- clinical data
- digital health
- government
---
