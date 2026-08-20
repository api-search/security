---
api_specs:
- filename: inngest-account-api-openapi.yml
  format: yaml
  label: Inngest Account API
  slug: inngest-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-account-api-openapi.yml
- filename: inngest-apps-api-openapi.yml
  format: yaml
  label: Inngest Apps API
  slug: inngest-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-apps-api-openapi.yml
- filename: inngest-environments-api-openapi.yml
  format: yaml
  label: Inngest Environments API
  slug: inngest-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-environments-api-openapi.yml
- filename: inngest-events-api-openapi.yml
  format: yaml
  label: Inngest Events API
  slug: inngest-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-events-api-openapi.yml
- filename: inngest-functions-api-openapi.yml
  format: yaml
  label: Inngest Functions API
  slug: inngest-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-functions-api-openapi.yml
- filename: inngest-keys-api-openapi.yml
  format: yaml
  label: Inngest Keys API
  slug: inngest-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-keys-api-openapi.yml
- filename: inngest-runs-api-openapi.yml
  format: yaml
  label: Inngest Runs API
  slug: inngest-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-runs-api-openapi.yml
- filename: inngest-webhooks-api-openapi.yml
  format: yaml
  label: Inngest Webhooks API
  slug: inngest-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/openapi/inngest-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inngest.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: inn.gs
  spf: false
hosts:
- cert_expires: Sep 26 16:21:46 2026 GMT
  host: www.inngest.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.inngest.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: inn.gs
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inngest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inngest, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inngest
provider_slug: inngest
slug: inngest-domain-security
source_filename: inngest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inngest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:21:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.inngest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\n- host: inn.gs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: inngest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: inn.gs\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inngest/refs/heads/main/security/inngest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- AgentKit
- Background Jobs
- Connect
- Cron Jobs
- Dev Server
- Durable Endpoints
- Durable Execution
- Event-Driven
- Insights
- Orchestration
- Queues
- Real-Time
- Self-Hosting
- Serverless
- Signals
- Step Functions
- Webhook
- Workflows
---
