---
api_specs:
- filename: flexpa-access-tokens-api-openapi.yml
  format: yaml
  label: Flexpa Access Tokens API
  slug: flexpa-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-access-tokens-api-openapi.yml
- filename: flexpa-claims-data-api-openapi.yml
  format: yaml
  label: Flexpa Claims Data API
  slug: flexpa-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-claims-data-api-openapi.yml
- filename: flexpa-fhir-api-openapi.yml
  format: yaml
  label: Flexpa FHIR API
  slug: flexpa-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-fhir-api-openapi.yml
- filename: flexpa-link-api-openapi.yml
  format: yaml
  label: Flexpa Link API
  slug: flexpa-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-link-api-openapi.yml
certifications:
- SOC 2 (published as "SOC II")
- HIPAA
- CARIN Alliance Code of Conduct
description: ''
kind: trust-center
layout: security
name: Flexpa Trust Center
name_suffix: Trust Center
overview: Flexpa maintains a public trust center documenting SOC 2 (published as "SOC II"), HIPAA, and CARIN Alliance Code of Conduct compliance.
provider_name: Flexpa
provider_slug: flexpa
slug: flexpa-trust-center
source_filename: flexpa-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://security.flexpa.com\nprovider: Flexpa\nproviderId: flexpa\ntrust_center:\n  url: https://security.flexpa.com\n  http_status: 200\n  title: Trust center\n  machine_readable: false\n  note: >-\n    A dedicated trust-centre subdomain is served, but it is a client-rendered\n    single-page app - the HTML shell carries only <title>Trust center</title>, and\n    the same shell is returned for every path including\n    /.well-known/security.txt and /api/*. No certification documents, subprocessor\n    list or NDA-gated request flow could be read without executing JavaScript.\n  probed: '2026-08-14'\ncertifications:\n- name: SOC 2 (published as \"SOC II\")\n  status: claimed\n  evidence_url: https://my.flexpa.com\n  report_available: unknown\n- name: HIPAA\n  status: claimed\n  evidence_url: https://my.flexpa.com\n  note: Flexpa states it is not a HIPAA covered entity; it may act as a business associate.\n- name: CARIN Alliance\
  \ Code of Conduct\n  status: signatory\n  evidence_url: https://www.flexpa.com/carin-code-of-conduct\ncontacts:\n  privacy: privacy@flexpa.com\n  support: support@flexpa.com\n  security: null\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/security/flexpa-trust-center.yml
summary_line: SOC 2 (published as "SOC II"), HIPAA, CARIN Alliance Code of Conduct
tags:
- Healthcare
- FHIR
- Patient Access
- Claims Data
- Health Insurance
trust_url: ''
---
