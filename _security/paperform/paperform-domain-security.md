---
api_specs:
- filename: paperform-coupons-api-openapi.yml
  format: yaml
  label: Paperform Coupons API
  slug: paperform-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-coupons-api-openapi.yml
- filename: paperform-files-api-openapi.yml
  format: yaml
  label: Paperform Files API
  slug: paperform-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-files-api-openapi.yml
- filename: paperform-form-fields-api-openapi.yml
  format: yaml
  label: Paperform Form Fields API
  slug: paperform-form-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-form-fields-api-openapi.yml
- filename: paperform-forms-api-openapi.yml
  format: yaml
  label: Paperform Forms API
  slug: paperform-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-forms-api-openapi.yml
- filename: paperform-papersign-documents-api-openapi.yml
  format: yaml
  label: Paperform Papersign Documents API
  slug: paperform-papersign-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-papersign-documents-api-openapi.yml
- filename: paperform-papersign-folders-api-openapi.yml
  format: yaml
  label: Paperform Papersign Folders API
  slug: paperform-papersign-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-papersign-folders-api-openapi.yml
- filename: paperform-papersign-spaces-api-openapi.yml
  format: yaml
  label: Paperform Papersign Spaces API
  slug: paperform-papersign-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-papersign-spaces-api-openapi.yml
- filename: paperform-papersign-webhooks-api-openapi.yml
  format: yaml
  label: Paperform Papersign Webhooks API
  slug: paperform-papersign-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-papersign-webhooks-api-openapi.yml
- filename: paperform-partial-submissions-api-openapi.yml
  format: yaml
  label: Paperform Partial Submissions API
  slug: paperform-partial-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-partial-submissions-api-openapi.yml
- filename: paperform-products-api-openapi.yml
  format: yaml
  label: Paperform Products API
  slug: paperform-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-products-api-openapi.yml
- filename: paperform-spaces-api-openapi.yml
  format: yaml
  label: Paperform Spaces API
  slug: paperform-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-spaces-api-openapi.yml
- filename: paperform-submissions-api-openapi.yml
  format: yaml
  label: Paperform Submissions API
  slug: paperform-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-submissions-api-openapi.yml
- filename: paperform-translations-api-openapi.yml
  format: yaml
  label: Paperform Translations API
  slug: paperform-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-translations-api-openapi.yml
- filename: paperform-webhooks-api-openapi.yml
  format: yaml
  label: Paperform Webhooks API
  slug: paperform-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/openapi/paperform-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: paperform.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: paperform.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: paperform.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: api.paperform.co
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Paperform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paperform, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Paperform
provider_slug: paperform
slug: paperform-domain-security
source_filename: paperform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paperform.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\n- host: paperform.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paperform.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: paperform.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperform/refs/heads/main/security/paperform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Forms
- Payments
- Submissions
- Surveys
- E-Signature
- Webhook
- No-Code
---
