---
api_specs:
- filename: sun-life-authorize-api-openapi.yml
  format: yaml
  label: Sun Life Authorize API
  slug: sun-life-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-authorize-api-openapi.yml
- filename: sun-life-callback-api-openapi.yml
  format: yaml
  label: Sun Life Callback API
  slug: sun-life-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-callback-api-openapi.yml
- filename: sun-life-coverage-api-openapi.yml
  format: yaml
  label: Sun Life Coverage API
  slug: sun-life-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-coverage-api-openapi.yml
- filename: sun-life-endpoint-api-openapi.yml
  format: yaml
  label: Sun Life Endpoint API
  slug: sun-life-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-endpoint-api-openapi.yml
- filename: sun-life-healthcareservice-api-openapi.yml
  format: yaml
  label: Sun Life Healthcare Service API
  slug: sun-life-healthcareservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-healthcareservice-api-openapi.yml
- filename: sun-life-insuranceplan-api-openapi.yml
  format: yaml
  label: Sun Life Insurance Plan API
  slug: sun-life-insuranceplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-insuranceplan-api-openapi.yml
- filename: sun-life-location-api-openapi.yml
  format: yaml
  label: Sun Life Location API
  slug: sun-life-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-location-api-openapi.yml
- filename: sun-life-metadata-api-openapi.yml
  format: yaml
  label: Sun Life Metadata API
  slug: sun-life-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-metadata-api-openapi.yml
- filename: sun-life-organization-api-openapi.yml
  format: yaml
  label: Sun Life Organization API
  slug: sun-life-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-organization-api-openapi.yml
- filename: sun-life-patient-api-openapi.yml
  format: yaml
  label: Sun Life Patient API
  slug: sun-life-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-patient-api-openapi.yml
- filename: sun-life-practitioner-api-openapi.yml
  format: yaml
  label: Sun Life Practitioner API
  slug: sun-life-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-practitioner-api-openapi.yml
- filename: sun-life-practitionerrole-api-openapi.yml
  format: yaml
  label: Sun Life Practitioner Role API
  slug: sun-life-practitionerrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-practitionerrole-api-openapi.yml
- filename: sun-life-relatedperson-api-openapi.yml
  format: yaml
  label: Sun Life Related Person API
  slug: sun-life-relatedperson-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-relatedperson-api-openapi.yml
- filename: sun-life-token-api-openapi.yml
  format: yaml
  label: Sun Life Token API
  slug: sun-life-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-token-api-openapi.yml
- filename: sun-life-tokenhook-api-openapi.yml
  format: yaml
  label: Sun Life Tokenhook API
  slug: sun-life-tokenhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-tokenhook-api-openapi.yml
- filename: sun-life-well-known-api-openapi.yml
  format: yaml
  label: Sun Life .well Known API
  slug: sun-life-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sunlife.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dentaquest.com
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: www.sunlife.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.dentaquest.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.deltadentalma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sun Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sun Life, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sun Life
provider_slug: sun-life
slug: sun-life-domain-security
source_filename: sun-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sunlife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dentaquest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\n- host: api.deltadentalma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sunlife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dentaquest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/security/sun-life-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Group Benefits
- Dental Insurance
- Disability
- Wealth Management
- Financial-Services
- Carrier
- FHIR
- Patient Access
- Provider Directory
- Healthcare Interoperability
- CMS-9115-F
- DentaQuest
- SMART on FHIR
- Dental Benefits
---
