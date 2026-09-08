---
api_specs:
- filename: centene-fhir-patient-access-openapi.json
  format: json
  label: Centene FHIR Patient Access API
  slug: centene-fhir-patient-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-fhir-patient-access-openapi.json
- filename: centene-fhir-provider-directory-openapi.json
  format: json
  label: Centene FHIR Provider Directory API
  slug: centene-fhir-provider-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-fhir-provider-directory-openapi.json
- filename: centene-provider-rtr-fhir-pdex-openapi.json
  format: json
  label: Centene Provider RTR - FHIR PDEX Directory API
  slug: centene-fhir-pdex-rtr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-rtr-fhir-pdex-openapi.json
- filename: centene-provider-rtr-demographics-openapi.json
  format: json
  label: Centene Provider RTR Demographics API
  slug: centene-provider-rtr-demographics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-rtr-demographics-openapi.json
- filename: centene-pces-openapi.yaml
  format: yaml
  label: Centene Provider Carrier Entity Search (PCES) API
  slug: centene-pces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-pces-openapi.yaml
- filename: centene-pces-extract-openapi.yaml
  format: yaml
  label: Centene Provider Carrier Entity Search (PCES) Extract API
  slug: centene-pces-extract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-pces-extract-openapi.yaml
- filename: centene-provider-search-suggest-openapi.yaml
  format: yaml
  label: Centene Provider Search Suggest API
  slug: centene-provider-search-suggest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-search-suggest-openapi.yaml
- filename: centene-product-mapping-v2-openapi.yaml
  format: yaml
  label: Centene Product Mapping V2 API
  slug: centene-product-mapping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-product-mapping-v2-openapi.yaml
- filename: centene-edi-core-realtime-openapi.json
  format: json
  label: Centene LWC EDI CORE Real Time Service
  slug: centene-edi-core-realtime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-edi-core-realtime-openapi.json
- filename: centene-ccm-communication-openapi.json
  format: json
  label: Centene CCM Communication API
  slug: centene-ccm-communication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-ccm-communication-openapi.json
- filename: centene-ccm-sms-userresponse-openapi.json
  format: json
  label: Centene CCM SMS User Response Webhook
  slug: centene-ccm-sms-userresponse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-ccm-sms-userresponse-openapi.json
- filename: centene-healow-health-openapi.yaml
  format: yaml
  label: Centene Healow Health API
  slug: centene-healow-health
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-healow-health-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: centene.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.centene.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: partners.centene.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: dev-int-api-gw.centene.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Centene Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centene, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Centene
provider_slug: centene
slug: centene-domain-security
source_filename: centene-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partners.centene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev-int-api-gw.centene.com\n  https: false\ndomains:\n- domain: centene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/security/centene-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Insurance
- Managed Care
- FHIR
- HL7
- CMS Interoperability
- Patient Access
- Provider Directory
- Payer
- Medicaid
- Medicare
- Interoperability
- SMART on FHIR
- PDEX
- CARIN Blue Button
- US Core
- Formulary
- X12
- EDI
- Fortune 500
---
