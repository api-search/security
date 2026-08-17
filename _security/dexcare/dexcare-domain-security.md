---
api_specs:
- filename: dexcare-visit-service-openapi.yml
  format: yaml
  label: DexCare Visit Service API
  slug: dexcare-visit-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-visit-service-openapi.yml
- filename: dexcare-care-options-openapi.yml
  format: yaml
  label: DexCare Care Options API
  slug: dexcare-care-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-care-options-openapi.yml
- filename: dexcare-slots-availability-openapi.yml
  format: yaml
  label: DexCare Slots Availability API
  slug: dexcare-slots-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-slots-availability-openapi.yml
- filename: dexcare-visit-booking-openapi.yml
  format: yaml
  label: DexCare Visit Booking API
  slug: dexcare-visit-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-visit-booking-openapi.yml
- filename: dexcare-omni-search-openapi.yml
  format: yaml
  label: DexCare Omni Search API
  slug: dexcare-omni-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-omni-search-openapi.yml
- filename: dexcare-provider-data-management-openapi.yml
  format: yaml
  label: DexCare Provider Data Management API
  slug: dexcare-provider-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/openapi/dexcare-provider-data-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dexcare.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dexcarehealth.com
  spf: true
hosts:
- cert_expires: Sep 24 13:01:15 2026 GMT
  host: dexcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 03:58:49 2026 GMT
  host: developers.dexcarehealth.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: api.care.dexcarehealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Dexcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DexCare, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DexCare
provider_slug: dexcare
slug: dexcare-domain-security
source_filename: dexcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dexcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:01:15 2026 GMT\n  hsts: false\n- host: developers.dexcarehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:58:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.care.dexcarehealth.com\n  https: false\ndomains:\n- domain: dexcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dexcarehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexcare/refs/heads/main/security/dexcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health IT
- Patient Access
- Scheduling
- Virtual Care
- Telehealth
- Care Navigation
- Provider Data
- Search
- SDK
---
