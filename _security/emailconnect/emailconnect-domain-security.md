---
api_specs:
- filename: emailconnect-api-v1-emails-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI API v1 - Emails API
  slug: emailconnect-api-v1-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-api-v1-emails-api-openapi.yml
- filename: emailconnect-api-v1-logs-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI API v1 - Logs API
  slug: emailconnect-api-v1-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-api-v1-logs-api-openapi.yml
- filename: emailconnect-api-v1-metrics-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI API v1 - Metrics API
  slug: emailconnect-api-v1-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-api-v1-metrics-api-openapi.yml
- filename: emailconnect-user-aliases-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI User Aliases API
  slug: emailconnect-user-aliases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-user-aliases-api-openapi.yml
- filename: emailconnect-user-domains-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI User Domains API
  slug: emailconnect-user-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-user-domains-api-openapi.yml
- filename: emailconnect-user-webhooks-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI User Webhooks API
  slug: emailconnect-user-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-user-webhooks-api-openapi.yml
- filename: emailconnect-webhook-alias-api-openapi.yml
  format: yaml
  label: EmailConnect by XADI Webhook Alias API
  slug: emailconnect-webhook-alias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/openapi/emailconnect-webhook-alias-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@emailconnect.eu"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: emailconnect.eu
  spf: true
hosts:
- cert_expires: Dec  3 22:17:42 2026 GMT
  host: emailconnect.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Emailconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailConnect by XADI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: EmailConnect by XADI
provider_slug: emailconnect
slug: emailconnect-domain-security
source_filename: emailconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailconnect.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 22:17:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emailconnect.eu\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@emailconnect.eu\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailconnect/refs/heads/main/security/emailconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- Webhook
- EU
- Compliance
---
