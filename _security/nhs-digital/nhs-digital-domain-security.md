---
api_specs:
- filename: nhs-digital-booking-api-openapi.yml
  format: yaml
  label: NHS Digital Booking API
  slug: nhs-digital-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-booking-api-openapi.yml
- filename: nhs-digital-communication-api-openapi.yml
  format: yaml
  label: NHS Digital communication API
  slug: nhs-digital-communication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-communication-api-openapi.yml
- filename: nhs-digital-message-api-openapi.yml
  format: yaml
  label: NHS Digital Message API
  slug: nhs-digital-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-message-api-openapi.yml
- filename: nhs-digital-metadata-api-openapi.yml
  format: yaml
  label: NHS Digital Metadata API
  slug: nhs-digital-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-metadata-api-openapi.yml
- filename: nhs-digital-r4-api-openapi.yml
  format: yaml
  label: NHS Digital R4 API
  slug: nhs-digital-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-r4-api-openapi.yml
- filename: nhs-digital-referral-api-openapi.yml
  format: yaml
  label: NHS Digital Referral API
  slug: nhs-digital-referral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-referral-api-openapi.yml
- filename: nhs-digital-slots-api-openapi.yml
  format: yaml
  label: NHS Digital Slots API
  slug: nhs-digital-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-slots-api-openapi.yml
- filename: nhs-digital-stu3-api-openapi.yml
  format: yaml
  label: NHS Digital STU3 API
  slug: nhs-digital-stu3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-digital/refs/heads/main/openapi/nhs-digital-stu3-api-openapi.yml
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
- Health
- FHIR
- UK
- patient demographics
- prescriptions
- Referrals
- clinical data
- digital health
- government
---
