---
api_specs:
- filename: sendmux-ai-billing-api-openapi.yml
  format: yaml
  label: sendmux-ai Billing API
  slug: sendmux-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-billing-api-openapi.yml
- filename: sendmux-ai-connection-api-openapi.yml
  format: yaml
  label: sendmux-ai Connection API
  slug: sendmux-ai-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-connection-api-openapi.yml
- filename: sendmux-ai-domain-filters-api-openapi.yml
  format: yaml
  label: sendmux-ai Domain Filters API
  slug: sendmux-ai-domain-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-domain-filters-api-openapi.yml
- filename: sendmux-ai-domains-api-openapi.yml
  format: yaml
  label: sendmux-ai Domains API
  slug: sendmux-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-domains-api-openapi.yml
- filename: sendmux-ai-emails-api-openapi.yml
  format: yaml
  label: sendmux-ai Emails API
  slug: sendmux-ai-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-emails-api-openapi.yml
- filename: sendmux-ai-inboxes-api-openapi.yml
  format: yaml
  label: sendmux-ai Inboxes API
  slug: sendmux-ai-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-inboxes-api-openapi.yml
- filename: sendmux-ai-mailbox-api-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailbox API
  slug: sendmux-ai-mailbox-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailbox-api-api-openapi.yml
- filename: sendmux-ai-mailbox-filters-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailbox Filters API
  slug: sendmux-ai-mailbox-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailbox-filters-api-openapi.yml
- filename: sendmux-ai-mailboxes-api-openapi.yml
  format: yaml
  label: sendmux-ai Mailboxes API
  slug: sendmux-ai-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-mailboxes-api-openapi.yml
- filename: sendmux-ai-sending-accounts-api-openapi.yml
  format: yaml
  label: sendmux-ai Sending accounts API
  slug: sendmux-ai-sending-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-sending-accounts-api-openapi.yml
- filename: sendmux-ai-webhooks-api-openapi.yml
  format: yaml
  label: sendmux-ai Webhooks API
  slug: sendmux-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendmux-ai/openapi/sendmux-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sendmux.ai
  spf: true
hosts:
- cert_expires: Jan 12 06:46:46 2027 GMT
  host: sendmux.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sendmux Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sendmux-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: sendmux-ai
provider_slug: sendmux-ai
slug: sendmux-ai-domain-security
source_filename: sendmux-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendmux.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 06:46:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sendmux.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sendmux-ai/security/sendmux-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- AI
- Agents
- Integration
---
