---
api_specs:
- filename: truepill-insurance-api-openapi.yml
  format: yaml
  label: Truepill Insurance API
  slug: truepill-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-insurance-api-openapi.yml
- filename: truepill-patients-api-openapi.yml
  format: yaml
  label: Truepill Patients API
  slug: truepill-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-patients-api-openapi.yml
- filename: truepill-prescriptions-api-openapi.yml
  format: yaml
  label: Truepill Prescriptions API
  slug: truepill-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-prescriptions-api-openapi.yml
- filename: truepill-transfers-api-openapi.yml
  format: yaml
  label: Truepill Transfers API
  slug: truepill-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-transfers-api-openapi.yml
- filename: truepill-webhooks-api-openapi.yml
  format: yaml
  label: Truepill Webhooks API
  slug: truepill-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-webhooks-api-openapi.yml
- filename: truepill-fulfillment-api-openapi.yml
  format: yaml
  label: Truepill Fulfillment API
  slug: truepill-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-fulfillment-api-openapi.yml
- filename: truepill-consults-api-openapi.yml
  format: yaml
  label: Truepill Consults API
  slug: truepill-consults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-consults-api-openapi.yml
- filename: truepill-diagnostics-api-openapi.yml
  format: yaml
  label: Truepill Diagnostics API
  slug: truepill-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-diagnostics-api-openapi.yml
- filename: truepill-media-api-openapi.yml
  format: yaml
  label: Truepill Media API
  slug: truepill-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/openapi/truepill-media-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: truepill.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fuzehealth.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.truepill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: rxdocs.fuzehealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: rxapi.fuzehealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truepill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truepill, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Truepill
provider_slug: truepill
slug: truepill-domain-security
source_filename: truepill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truepill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n- host: rxdocs.fuzehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: rxapi.fuzehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: truepill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fuzehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truepill/refs/heads/main/security/truepill-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pharmacy
- Healthcare
- Prescription Fulfillment
- Telehealth
- Diagnostics
- Insurance
- Copay Adjudication
- Prior Authorization
- Electronic Prescribing
- Pharmacy Transfers
- Webhooks
- HIPAA
---
