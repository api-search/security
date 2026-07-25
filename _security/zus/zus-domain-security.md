---
api_specs:
- filename: zus-auth-api-openapi.yml
  format: yaml
  label: Zus Health Auth API
  slug: zus-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-auth-api-openapi.yml
- filename: zus-documents-api-openapi.yml
  format: yaml
  label: Zus Health Documents API
  slug: zus-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-documents-api-openapi.yml
- filename: zus-fhir-api-openapi.yml
  format: yaml
  label: Zus Health FHIR API
  slug: zus-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-fhir-api-openapi.yml
- filename: zus-patient-api-openapi.yml
  format: yaml
  label: Zus Health Patient API
  slug: zus-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-patient-api-openapi.yml
- filename: zus-patient-history-api-openapi.yml
  format: yaml
  label: Zus Health Patient History API
  slug: zus-patient-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/openapi/zus-patient-history-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zushealth.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zusapi.com
  spf: false
hosts:
- cert_expires: Sep 11 00:14:22 2026 GMT
  host: zushealth.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 09:33:49 2026 GMT
  host: docs.zushealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.zusapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zus Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zus Health
provider_slug: zus
slug: zus-domain-security
source_filename: zus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zushealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:14:22 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.zushealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:33:49 2026 GMT\n  hsts: null\n- host: api.zusapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zushealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zusapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zus/refs/heads/main/security/zus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- FHIR
- Interoperability
- Patient Data
- Healthcare
---
