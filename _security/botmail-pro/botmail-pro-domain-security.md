---
api_specs:
- filename: botmail-pro-account-api-openapi.yml
  format: yaml
  label: Botmail Account API
  slug: botmail-pro-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-account-api-openapi.yml
- filename: botmail-pro-billing-api-openapi.yml
  format: yaml
  label: Botmail Billing API
  slug: botmail-pro-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-billing-api-openapi.yml
- filename: botmail-pro-claim-api-openapi.yml
  format: yaml
  label: Botmail Claim API
  slug: botmail-pro-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-claim-api-openapi.yml
- filename: botmail-pro-events-api-openapi.yml
  format: yaml
  label: Botmail Events API
  slug: botmail-pro-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-events-api-openapi.yml
- filename: botmail-pro-keys-api-openapi.yml
  format: yaml
  label: Botmail Keys API
  slug: botmail-pro-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-keys-api-openapi.yml
- filename: botmail-pro-mail-api-openapi.yml
  format: yaml
  label: Botmail Mail API
  slug: botmail-pro-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-mail-api-openapi.yml
- filename: botmail-pro-mailboxes-api-openapi.yml
  format: yaml
  label: Botmail Mailboxes API
  slug: botmail-pro-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-mailboxes-api-openapi.yml
- filename: botmail-pro-meta-api-openapi.yml
  format: yaml
  label: Botmail Meta API
  slug: botmail-pro-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-meta-api-openapi.yml
- filename: botmail-pro-send-api-openapi.yml
  format: yaml
  label: Botmail Send API
  slug: botmail-pro-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-send-api-openapi.yml
- filename: botmail-pro-webhooks-api-openapi.yml
  format: yaml
  label: Botmail Webhooks API
  slug: botmail-pro-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botmail-pro/openapi/botmail-pro-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: botmail.pro
  spf: false
hosts:
- cert_expires: Jan  8 14:06:45 2027 GMT
  host: botmail.pro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Botmail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Botmail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Botmail
provider_slug: botmail-pro
slug: botmail-pro-domain-security
source_filename: botmail-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botmail.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 14:06:45 2027 GMT\n  hsts: false\ndomains:\n- domain: botmail.pro\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/botmail-pro/security/botmail-pro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Email
- Messaging
- Automation
- Botmail
---
