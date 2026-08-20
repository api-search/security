---
api_specs:
- filename: wufoo-webhooks-asyncapi.yml
  format: yaml
  label: Wufoo Webhooks
  slug: wufoo-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/asyncapi/wufoo-webhooks-asyncapi.yml
- filename: wufoo-comments-api-openapi.yml
  format: yaml
  label: Wufoo Comments API
  slug: wufoo-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-comments-api-openapi.yml
- filename: wufoo-entries-api-openapi.yml
  format: yaml
  label: Wufoo Entries API
  slug: wufoo-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-entries-api-openapi.yml
- filename: wufoo-fields-api-openapi.yml
  format: yaml
  label: Wufoo Fields API
  slug: wufoo-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-fields-api-openapi.yml
- filename: wufoo-forms-api-openapi.yml
  format: yaml
  label: Wufoo Forms API
  slug: wufoo-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-forms-api-openapi.yml
- filename: wufoo-login-api-openapi.yml
  format: yaml
  label: Wufoo Login API
  slug: wufoo-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-login-api-openapi.yml
- filename: wufoo-reports-api-openapi.yml
  format: yaml
  label: Wufoo Reports API
  slug: wufoo-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-reports-api-openapi.yml
- filename: wufoo-users-api-openapi.yml
  format: yaml
  label: Wufoo Users API
  slug: wufoo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-users-api-openapi.yml
- filename: wufoo-webhooks-api-openapi.yml
  format: yaml
  label: Wufoo Webhooks API
  slug: wufoo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-webhooks-api-openapi.yml
- filename: wufoo-widgets-api-openapi.yml
  format: yaml
  label: Wufoo Widgets API
  slug: wufoo-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-widgets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wufoo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: surveymonkey.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: www.wufoo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: help.surveymonkey.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wufoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wufoo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wufoo
provider_slug: wufoo
slug: wufoo-domain-security
source_filename: wufoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wufoo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.surveymonkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wufoo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: surveymonkey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/security/wufoo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Form Builder
- Surveys
- Data Collection
- Webhook
- Payments
- SurveyMonkey
---
