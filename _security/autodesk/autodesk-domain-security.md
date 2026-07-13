---
api_specs:
- filename: autodesk-authentication-openapi.yml
  format: yaml
  label: Autodesk Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-authentication-openapi.yml
- filename: autodesk-data-management-openapi.yml
  format: yaml
  label: Autodesk Data Management API
  slug: data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-data-management-openapi.yml
- filename: autodesk-model-derivative-openapi.yml
  format: yaml
  label: Autodesk Model Derivative API
  slug: model-derivative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-model-derivative-openapi.yml
- filename: autodesk-design-automation-openapi.yml
  format: yaml
  label: Autodesk Design Automation API
  slug: design-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-design-automation-openapi.yml
- filename: autodesk-webhooks-openapi.yml
  format: yaml
  label: Autodesk Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-webhooks-openapi.yml
- filename: autodesk-reality-capture-openapi.yml
  format: yaml
  label: Autodesk Reality Capture API
  slug: reality-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-reality-capture-openapi.yml
- filename: autodesk-sustainability-data-openapi.yml
  format: yaml
  label: Autodesk Sustainability Data API
  slug: sustainability-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-sustainability-data-openapi.yml
- filename: autodesk-parameters-openapi.yml
  format: yaml
  label: Autodesk Parameters API
  slug: parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-parameters-openapi.yml
- filename: autodesk-tandem-data-openapi.yml
  format: yaml
  label: Autodesk Tandem Data API
  slug: tandem-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-tandem-data-openapi.yml
- filename: autodesk-flow-graph-engine-openapi.yml
  format: yaml
  label: Autodesk Flow Graph Engine API
  slug: flow-graph-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-flow-graph-engine-openapi.yml
- filename: autodesk-acc-account-admin-openapi.yml
  format: yaml
  label: Autodesk ACC Account Admin API
  slug: acc-account-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-acc-account-admin-openapi.yml
- filename: autodesk-bim360-openapi.yml
  format: yaml
  label: Autodesk BIM 360 API
  slug: bim-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/openapi/autodesk-bim360-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: autodesk.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: aps.autodesk.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.autodesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: developer.api.autodesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autodesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autodesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Autodesk
provider_slug: autodesk
slug: autodesk-domain-security
source_filename: autodesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aps.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\n- host: developer.api.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: autodesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk/refs/heads/main/security/autodesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fortune 1000
- 3D Modeling
- Architecture
- BIM
- CAD
- Construction
- Design
- Digital Twins
- Engineering
- Manufacturing
- Media and Entertainment
- Sustainability
---
