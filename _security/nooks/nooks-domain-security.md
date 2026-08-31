---
api_specs:
- filename: nooks-accounts-api-openapi.yml
  format: yaml
  label: Nooks Accounts API
  slug: nooks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-accounts-api-openapi.yml
- filename: nooks-calldispositions-api-openapi.yml
  format: yaml
  label: Nooks Call Dispositions API
  slug: nooks-calldispositions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-calldispositions-api-openapi.yml
- filename: nooks-calls-api-openapi.yml
  format: yaml
  label: Nooks Calls API
  slug: nooks-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-calls-api-openapi.yml
- filename: nooks-emails-api-openapi.yml
  format: yaml
  label: Nooks Emails API
  slug: nooks-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-emails-api-openapi.yml
- filename: nooks-emailtemplates-api-openapi.yml
  format: yaml
  label: Nooks Email Templates API
  slug: nooks-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-emailtemplates-api-openapi.yml
- filename: nooks-introspection-api-openapi.yml
  format: yaml
  label: Nooks Introspection API
  slug: nooks-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-introspection-api-openapi.yml
- filename: nooks-mailboxes-api-openapi.yml
  format: yaml
  label: Nooks Mailboxes API
  slug: nooks-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-mailboxes-api-openapi.yml
- filename: nooks-nooks-sequencing-api-api-openapi.yml
  format: yaml
  label: Nooks Nooks Sequencing API
  slug: nooks-nooks-sequencing-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-nooks-sequencing-api-api-openapi.yml
- filename: nooks-notes-api-openapi.yml
  format: yaml
  label: Nooks Notes API
  slug: nooks-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-notes-api-openapi.yml
- filename: nooks-prospects-api-openapi.yml
  format: yaml
  label: Nooks Prospects API
  slug: nooks-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-prospects-api-openapi.yml
- filename: nooks-sequences-api-openapi.yml
  format: yaml
  label: Nooks Sequences API
  slug: nooks-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequences-api-openapi.yml
- filename: nooks-sequencestates-api-openapi.yml
  format: yaml
  label: Nooks Sequence States API
  slug: nooks-sequencestates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencestates-api-openapi.yml
- filename: nooks-sequencesteps-api-openapi.yml
  format: yaml
  label: Nooks Sequence Steps API
  slug: nooks-sequencesteps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencesteps-api-openapi.yml
- filename: nooks-tasks-api-openapi.yml
  format: yaml
  label: Nooks Tasks API
  slug: nooks-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-tasks-api-openapi.yml
- filename: nooks-users-api-openapi.yml
  format: yaml
  label: Nooks Users API
  slug: nooks-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nooks.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nooks.in
  spf: true
hosts:
- cert_expires: Nov  6 22:41:01 2026 GMT
  host: www.nooks.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:21:48 2026 GMT
  host: developer.nooks.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 06:47:29 2026 GMT
  host: partner-api.nooks.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nooks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nooks
provider_slug: nooks
slug: nooks-domain-security
source_filename: nooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nooks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 22:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nooks.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:21:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-api.nooks.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:47:29 2026 GMT\n  hsts: null\ndomains:\n- domain: nooks.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nooks.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/security/nooks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Sales Engagement
- Sales Dialer
- AI SDR
- Outbound Sales
- Sales Coaching
- Revenue Operations
- Sales Sequencing
- CRM Integration
- Agents
- MCP
---
