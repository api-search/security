---
api_specs:
- filename: airslate-document-fields-api-openapi.yml
  format: yaml
  label: airSlate Document Fields API
  slug: airslate-document-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-document-fields-api-openapi.yml
- filename: airslate-document-groups-api-openapi.yml
  format: yaml
  label: airSlate Document Groups API
  slug: airslate-document-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-document-groups-api-openapi.yml
- filename: airslate-documents-api-openapi.yml
  format: yaml
  label: airSlate Documents API
  slug: airslate-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-documents-api-openapi.yml
- filename: airslate-embedded-api-openapi.yml
  format: yaml
  label: airSlate Embedded API
  slug: airslate-embedded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-embedded-api-openapi.yml
- filename: airslate-folders-api-openapi.yml
  format: yaml
  label: airSlate Folders API
  slug: airslate-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-folders-api-openapi.yml
- filename: airslate-invites-api-openapi.yml
  format: yaml
  label: airSlate Invites API
  slug: airslate-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-invites-api-openapi.yml
- filename: airslate-oauth-api-openapi.yml
  format: yaml
  label: airSlate OAuth API
  slug: airslate-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-oauth-api-openapi.yml
- filename: airslate-smart-fields-api-openapi.yml
  format: yaml
  label: airSlate Smart Fields API
  slug: airslate-smart-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-smart-fields-api-openapi.yml
- filename: airslate-templates-api-openapi.yml
  format: yaml
  label: airSlate Templates API
  slug: airslate-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-templates-api-openapi.yml
- filename: airslate-users-api-openapi.yml
  format: yaml
  label: airSlate Users API
  slug: airslate-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-users-api-openapi.yml
- filename: airslate-webhooks-api-openapi.yml
  format: yaml
  label: airSlate Webhooks API
  slug: airslate-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airslate.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signnow.com
  spf: true
hosts:
- cert_expires: Sep  4 18:29:10 2026 GMT
  host: www.airslate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 07:01:05 2026 GMT
  host: docs.signnow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 17:54:47 2026 GMT
  host: api.signnow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airslate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for airSlate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: airSlate
provider_slug: airslate
slug: airslate-domain-security
source_filename: airslate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airslate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 18:29:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.signnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:01:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.signnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 17:54:47 2026 GMT\n  hsts: null\ndomains:\n- domain: airslate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: signnow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/security/airslate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Automation
- eSignature
- Workflows
- PDF
- No-Code
- Artificial Intelligence
---
