---
api_specs:
- filename: siro-audit-api-openapi.yml
  format: yaml
  label: Siro Audit API
  slug: siro-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-audit-api-openapi.yml
- filename: siro-core-api-openapi.yml
  format: yaml
  label: Siro Core API
  slug: siro-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-core-api-openapi.yml
- filename: siro-folders-api-openapi.yml
  format: yaml
  label: Siro Folders API
  slug: siro-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-folders-api-openapi.yml
- filename: siro-integrations-api-openapi.yml
  format: yaml
  label: Siro Integrations API
  slug: siro-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-integrations-api-openapi.yml
- filename: siro-agents-api-openapi.yml
  format: yaml
  label: Siro Agents API
  slug: siro-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-agents-api-openapi.yml
- filename: siro-billing-graph-api-openapi.yml
  format: yaml
  label: Siro Billing Graph API
  slug: siro-billing-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-billing-graph-api-openapi.yml
- filename: siro-docs-api-openapi.yml
  format: yaml
  label: Siro Docs API
  slug: siro-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-docs-api-openapi.yml
- filename: siro-halftime-api-openapi.yml
  format: yaml
  label: Siro Halftime API
  slug: siro-halftime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-halftime-api-openapi.yml
- filename: siro-intercom-api-openapi.yml
  format: yaml
  label: Siro Intercom API
  slug: siro-intercom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-intercom-api-openapi.yml
- filename: siro-invoices-api-openapi.yml
  format: yaml
  label: Siro Invoices API
  slug: siro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-invoices-api-openapi.yml
- filename: siro-jobs-api-openapi.yml
  format: yaml
  label: Siro Jobs API
  slug: siro-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-jobs-api-openapi.yml
- filename: siro-licenses-api-openapi.yml
  format: yaml
  label: Siro Licenses API
  slug: siro-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-licenses-api-openapi.yml
- filename: siro-portal-api-openapi.yml
  format: yaml
  label: Siro Portal API
  slug: siro-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-portal-api-openapi.yml
- filename: siro-sessions-api-openapi.yml
  format: yaml
  label: Siro Sessions API
  slug: siro-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-sessions-api-openapi.yml
- filename: siro-subscription-api-openapi.yml
  format: yaml
  label: Siro Subscription API
  slug: siro-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-subscription-api-openapi.yml
- filename: siro-suggested-questions-api-openapi.yml
  format: yaml
  label: Siro Suggested Questions API
  slug: siro-suggested-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-suggested-questions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: siro.ai
  spf: true
hosts:
- cert_expires: Sep 12 05:45:56 2026 GMT
  host: siro.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 10:06:25 2026 GMT
  host: docs.siro.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 14:33:44 2026 GMT
  host: functions.siro.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Siro
provider_slug: siro
slug: siro-domain-security
source_filename: siro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:45:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.siro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:06:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: functions.siro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:33:44 2026 GMT\n  hsts: null\ndomains:\n- domain: siro.ai\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/security/siro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sales
- Sales Coaching
- Conversation Intelligence
- Field Sales
- CRM
- Artificial Intelligence
- Speech-to-Text
- Webhook
- Integration
---
