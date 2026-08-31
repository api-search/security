---
api_specs:
- filename: wellcare-health-plans-condition-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Condition API
  slug: wellcare-health-plans-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-condition-api-openapi.yml
- filename: wellcare-health-plans-coverage-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Coverage API
  slug: wellcare-health-plans-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-coverage-api-openapi.yml
- filename: wellcare-health-plans-encounter-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Encounter API
  slug: wellcare-health-plans-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-encounter-api-openapi.yml
- filename: wellcare-health-plans-explanation-of-benefits-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Explanation of Benefits API
  slug: wellcare-health-plans-explanation-of-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-explanation-of-benefits-api-openapi.yml
- filename: wellcare-health-plans-immunization-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Immunization API
  slug: wellcare-health-plans-immunization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-immunization-api-openapi.yml
- filename: wellcare-health-plans-insurance-plan-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Insurance Plan API
  slug: wellcare-health-plans-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-insurance-plan-api-openapi.yml
- filename: wellcare-health-plans-location-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Location API
  slug: wellcare-health-plans-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-location-api-openapi.yml
- filename: wellcare-health-plans-medication-request-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Medication Request API
  slug: wellcare-health-plans-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-medication-request-api-openapi.yml
- filename: wellcare-health-plans-observation-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Observation API
  slug: wellcare-health-plans-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-observation-api-openapi.yml
- filename: wellcare-health-plans-organization-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Organization API
  slug: wellcare-health-plans-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-organization-api-openapi.yml
- filename: wellcare-health-plans-patient-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Patient API
  slug: wellcare-health-plans-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-patient-api-openapi.yml
- filename: wellcare-health-plans-practitioner-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Practitioner API
  slug: wellcare-health-plans-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-practitioner-api-openapi.yml
- filename: wellcare-health-plans-practitioner-role-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Practitioner Role API
  slug: wellcare-health-plans-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-practitioner-role-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wellcare.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: centene.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.wellcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: partners.centene.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellcare Health Plans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WellCare Health Plans, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WellCare Health Plans
provider_slug: wellcare-health-plans
slug: wellcare-health-plans-domain-security
source_filename: wellcare-health-plans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wellcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partners.centene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wellcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: centene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/security/wellcare-health-plans-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
---
