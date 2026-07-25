---
api_specs:
- filename: nhs-e-referral-service-openapi.yaml
  format: yaml
  label: e-Referral Service (e-RS) - FHIR API
  slug: nhs-e-referral-service-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-e-referral-service-openapi.yaml
- filename: nhs-booking-and-referral-fhir-openapi.yaml
  format: yaml
  label: Booking and Referral Standard (BaRS) - FHIR API
  slug: nhs-booking-and-referral-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-booking-and-referral-fhir-openapi.yaml
- filename: nhs-immunisation-history-openapi.yaml
  format: yaml
  label: Immunisation History - FHIR API
  slug: nhs-immunisation-history-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-immunisation-history-openapi.yaml
- filename: nhs-organisation-data-service-fhir-r4-openapi.yaml
  format: yaml
  label: Organisation Data Service (ODS) - FHIR API
  slug: nhs-organisation-data-service-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-organisation-data-service-fhir-r4-openapi.yaml
- filename: nhs-app-openapi.yaml
  format: yaml
  label: NHS App API
  slug: nhs-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-app-openapi.yaml
- filename: nhs-communications-manager-openapi.yaml
  format: yaml
  label: NHS Notify (Communications Manager) API
  slug: nhs-notify-communications-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-communications-manager-openapi.yaml
- filename: nhs-service-search-openapi.yaml
  format: yaml
  label: Service Search (Directory of Healthcare Services) API
  slug: nhs-service-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/openapi/nhs-service-search-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhs.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dc4h.link
  spf: false
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
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: beta.ods.dc4h.link
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nhs England Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NHS England, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NHS England
provider_slug: nhs-england
slug: nhs-england-domain-security
source_filename: nhs-england-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digital.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:44 2026 GMT\n  hsts: null\n- host: api.service.nhs.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\n- host: beta.ods.dc4h.link\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nhs.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dc4h.link\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-england/refs/heads/main/security/nhs-england-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- United Kingdom
- National Health System
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Health Data
- e-Prescribing
- EHR
---
