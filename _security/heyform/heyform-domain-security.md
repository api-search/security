---
api_specs:
- filename: heyform-auth-api-openapi.yml
  format: yaml
  label: HeyForm Auth API
  slug: heyform-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-auth-api-openapi.yml
- filename: heyform-config-api-openapi.yml
  format: yaml
  label: HeyForm Config API
  slug: heyform-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-config-api-openapi.yml
- filename: heyform-forms-api-openapi.yml
  format: yaml
  label: HeyForm Forms API
  slug: heyform-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-forms-api-openapi.yml
- filename: heyform-graphql-api-openapi.yml
  format: yaml
  label: HeyForm GraphQL API
  slug: heyform-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-graphql-api-openapi.yml
- filename: heyform-images-api-openapi.yml
  format: yaml
  label: HeyForm Images API
  slug: heyform-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-images-api-openapi.yml
- filename: heyform-submissions-api-openapi.yml
  format: yaml
  label: HeyForm Submissions API
  slug: heyform-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-submissions-api-openapi.yml
- filename: heyform-upload-api-openapi.yml
  format: yaml
  label: HeyForm Upload API
  slug: heyform-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-upload-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heyform.net
  spf: true
hosts:
- cert_expires: Sep 19 15:12:26 2026 GMT
  host: heyform.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 13:11:47 2026 GMT
  host: docs.heyform.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.heyform.net
  https: false
kind: domain-security
layout: security
method: probed
name: Heyform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeyForm, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HeyForm
provider_slug: heyform
slug: heyform-domain-security
source_filename: heyform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heyform.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:12:26 2026 GMT\n  hsts: false\n- host: docs.heyform.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:11:47 2026 GMT\n  hsts: false\n- host: api.heyform.net\n  https: false\ndomains:\n- domain: heyform.net\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/security/heyform-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Forms
- Surveys
- Quizzes
- Polls
- Conversational Forms
- Open Source
- Webhooks
- No-Code
- Form Builder
- Self-Hosted
---
