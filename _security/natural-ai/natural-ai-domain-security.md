---
api_specs:
- filename: natural-ai-agent-keys-api-openapi.yml
  format: yaml
  label: Natural AI Agent Keys API
  slug: natural-ai-agent-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-agent-keys-api-openapi.yml
- filename: natural-ai-agents-api-openapi.yml
  format: yaml
  label: Natural AI Agents API
  slug: natural-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-agents-api-openapi.yml
- filename: natural-ai-api-keys-api-openapi.yml
  format: yaml
  label: Natural AI API Keys API
  slug: natural-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-api-keys-api-openapi.yml
- filename: natural-ai-approvals-api-openapi.yml
  format: yaml
  label: Natural AI Approvals API
  slug: natural-ai-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-approvals-api-openapi.yml
- filename: natural-ai-customers-api-openapi.yml
  format: yaml
  label: Natural AI Customers API
  slug: natural-ai-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-customers-api-openapi.yml
- filename: natural-ai-events-api-openapi.yml
  format: yaml
  label: Natural AI Events API
  slug: natural-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-events-api-openapi.yml
- filename: natural-ai-external-accounts-api-openapi.yml
  format: yaml
  label: Natural AI External Accounts API
  slug: natural-ai-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-external-accounts-api-openapi.yml
- filename: natural-ai-invitations-api-openapi.yml
  format: yaml
  label: Natural AI Invitations API
  slug: natural-ai-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-invitations-api-openapi.yml
- filename: natural-ai-parties-api-openapi.yml
  format: yaml
  label: Natural AI Parties API
  slug: natural-ai-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-parties-api-openapi.yml
- filename: natural-ai-paymentrequests-api-openapi.yml
  format: yaml
  label: Natural AI PaymentRequests API
  slug: natural-ai-paymentrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-paymentrequests-api-openapi.yml
- filename: natural-ai-payments-api-openapi.yml
  format: yaml
  label: Natural AI Payments API
  slug: natural-ai-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-payments-api-openapi.yml
- filename: natural-ai-transactions-api-openapi.yml
  format: yaml
  label: Natural AI Transactions API
  slug: natural-ai-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-transactions-api-openapi.yml
- filename: natural-ai-transfers-api-openapi.yml
  format: yaml
  label: Natural AI Transfers API
  slug: natural-ai-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-transfers-api-openapi.yml
- filename: natural-ai-wallets-api-openapi.yml
  format: yaml
  label: Natural AI Wallets API
  slug: natural-ai-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-wallets-api-openapi.yml
- filename: natural-ai-webhooks-api-openapi.yml
  format: yaml
  label: Natural AI Webhooks API
  slug: natural-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/openapi/natural-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: natural.com
  spf: true
hosts:
- cert_expires: Oct  5 21:02:56 2026 GMT
  host: www.natural.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:47:39 2026 GMT
  host: docs.natural.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.natural.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Natural Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natural AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Natural AI
provider_slug: natural-ai
slug: natural-ai-domain-security
source_filename: natural-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.natural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:02:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.natural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:47:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.natural.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: natural.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natural-ai/refs/heads/main/security/natural-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Payments
- Agents
- Fintech
- Money Movement
- Wallets
- Agentic Payments
- MCP
---
