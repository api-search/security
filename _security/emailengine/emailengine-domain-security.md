---
api_specs:
- filename: emailengine-account-api-openapi.yml
  format: yaml
  label: EmailEngine Account API
  slug: emailengine-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-account-api-openapi.yml
- filename: emailengine-accounts-api-openapi.yml
  format: yaml
  label: EmailEngine Accounts API
  slug: emailengine-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-accounts-api-openapi.yml
- filename: emailengine-autoconfig-api-openapi.yml
  format: yaml
  label: EmailEngine Autoconfig API
  slug: emailengine-autoconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-autoconfig-api-openapi.yml
- filename: emailengine-deliverytest-api-openapi.yml
  format: yaml
  label: EmailEngine Deliverytest API
  slug: emailengine-deliverytest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-deliverytest-api-openapi.yml
- filename: emailengine-gateways-api-openapi.yml
  format: yaml
  label: EmailEngine Gateways API
  slug: emailengine-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-gateways-api-openapi.yml
- filename: emailengine-license-api-openapi.yml
  format: yaml
  label: EmailEngine License API
  slug: emailengine-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-license-api-openapi.yml
- filename: emailengine-logs-api-openapi.yml
  format: yaml
  label: EmailEngine Logs API
  slug: emailengine-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-logs-api-openapi.yml
- filename: emailengine-oauth2-api-openapi.yml
  format: yaml
  label: EmailEngine Oauth2 API
  slug: emailengine-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-oauth2-api-openapi.yml
- filename: emailengine-outbox-api-openapi.yml
  format: yaml
  label: EmailEngine Outbox API
  slug: emailengine-outbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-outbox-api-openapi.yml
- filename: emailengine-stats-api-openapi.yml
  format: yaml
  label: EmailEngine Stats API
  slug: emailengine-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-stats-api-openapi.yml
- filename: emailengine-templates-api-openapi.yml
  format: yaml
  label: EmailEngine Templates API
  slug: emailengine-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-templates-api-openapi.yml
- filename: emailengine-tokens-api-openapi.yml
  format: yaml
  label: EmailEngine Tokens API
  slug: emailengine-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-tokens-api-openapi.yml
- filename: emailengine-webhookroutes-api-openapi.yml
  format: yaml
  label: EmailEngine Webhookroutes API
  slug: emailengine-webhookroutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-webhookroutes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emailengine.app
  spf: true
hosts:
- cert_expires: Aug 30 23:10:39 2026 GMT
  host: emailengine.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 16:22:24 2026 GMT
  host: api.emailengine.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emailengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailEngine, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EmailEngine
provider_slug: emailengine
slug: emailengine-domain-security
source_filename: emailengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailengine.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:10:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.emailengine.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 16:22:24 2026 GMT\n  hsts: false\ndomains:\n- domain: emailengine.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/security/emailengine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Email API
- IMAP
- SMTP
- Webhooks
---
