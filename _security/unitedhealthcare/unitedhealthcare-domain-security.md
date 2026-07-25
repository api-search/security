---
api_specs:
- filename: unitedhealthcare-claims-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Claims API
  slug: unitedhealthcare-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-claims-api-openapi.yml
- filename: unitedhealthcare-eligibility-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Eligibility API
  slug: unitedhealthcare-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-eligibility-api-openapi.yml
- filename: unitedhealthcare-formulary-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Formulary API
  slug: unitedhealthcare-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-formulary-api-openapi.yml
- filename: unitedhealthcare-patient-access-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Patient Access API
  slug: unitedhealthcare-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-patient-access-api-openapi.yml
- filename: unitedhealthcare-prior-authorization-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Prior Authorization API
  slug: unitedhealthcare-prior-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-prior-authorization-api-openapi.yml
- filename: unitedhealthcare-provider-directory-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Provider Directory API
  slug: unitedhealthcare-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-provider-directory-api-openapi.yml
- filename: unitedhealthcare-providers-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Providers API
  slug: unitedhealthcare-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-providers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uhcprovider.com
  spf: true
- caa:
  - 0 issuemail "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uhc.com
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: apimarketplace.uhcprovider.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.uhcprovider.com
  https: false
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.uhc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unitedhealthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UnitedHealthcare, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: UnitedHealthcare
provider_slug: unitedhealthcare
slug: unitedhealthcare-domain-security
source_filename: unitedhealthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apimarketplace.uhcprovider.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.uhcprovider.com\n  https: false\n- host: www.uhc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: uhcprovider.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: uhc.com\n  dnssec: true\n  caa:\n  - 0 issuemail \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/security/unitedhealthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health Insurance
- Healthcare
- FHIR
- Claims
- Eligibility
---
