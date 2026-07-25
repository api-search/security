---
api_specs:
- filename: nhs-api-codesystem-api-openapi.yml
  format: yaml
  label: NHS API CodeSystem API
  slug: nhs-api-codesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-codesystem-api-openapi.yml
- filename: nhs-api-list-id-api-openapi.yml
  format: yaml
  label: NHS API List{id} API
  slug: nhs-api-list-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-list-id-api-openapi.yml
- filename: nhs-api-metadata-api-openapi.yml
  format: yaml
  label: NHS API Metadata API
  slug: nhs-api-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-metadata-api-openapi.yml
- filename: nhs-api-organization-api-openapi.yml
  format: yaml
  label: NHS API Organization API
  slug: nhs-api-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-organization-api-openapi.yml
- filename: nhs-api-organizationaffiliation-api-openapi.yml
  format: yaml
  label: NHS API OrganizationAffiliation API
  slug: nhs-api-organizationaffiliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-organizationaffiliation-api-openapi.yml
- filename: nhs-api-r4-api-openapi.yml
  format: yaml
  label: NHS API R4 API
  slug: nhs-api-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-r4-api-openapi.yml
- filename: nhs-api-stu3-api-openapi.yml
  format: yaml
  label: NHS API STU3 API
  slug: nhs-api-stu3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-stu3-api-openapi.yml
- filename: nhs-api-valueset-api-openapi.yml
  format: yaml
  label: NHS API ValueSet API
  slug: nhs-api-valueset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-valueset-api-openapi.yml
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
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: auth.login.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nhs Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NHS API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NHS API
provider_slug: nhs-api
slug: nhs-api-domain-security
source_filename: nhs-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digital.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:44 2026 GMT\n  hsts: null\n- host: api.service.nhs.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\n- host: auth.login.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nhs.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/security/nhs-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- FHIR
- NHS
- UK
- HL7
- Electronic Prescriptions
- Patient Demographics
- GP Connect
- NHS Login
- Interoperability
---
