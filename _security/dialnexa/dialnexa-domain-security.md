---
api_specs:
- filename: dialnexa-agents-api-openapi.yml
  format: yaml
  label: DialNexa Agents API
  slug: dialnexa-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-agents-api-openapi.yml
- filename: dialnexa-batch-calls-api-openapi.yml
  format: yaml
  label: DialNexa Batch Calls API
  slug: dialnexa-batch-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-batch-calls-api-openapi.yml
- filename: dialnexa-calls-api-openapi.yml
  format: yaml
  label: DialNexa Calls API
  slug: dialnexa-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-calls-api-openapi.yml
- filename: dialnexa-knowledge-base-api-openapi.yml
  format: yaml
  label: DialNexa Knowledge Base API
  slug: dialnexa-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-knowledge-base-api-openapi.yml
- filename: dialnexa-languages-api-openapi.yml
  format: yaml
  label: DialNexa Languages API
  slug: dialnexa-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-languages-api-openapi.yml
- filename: dialnexa-llms-api-openapi.yml
  format: yaml
  label: DialNexa LL Ms API
  slug: dialnexa-llms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-llms-api-openapi.yml
- filename: dialnexa-organization-folders-api-openapi.yml
  format: yaml
  label: DialNexa Organization Folders API
  slug: dialnexa-organization-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-organization-folders-api-openapi.yml
- filename: dialnexa-phone-numbers-api-openapi.yml
  format: yaml
  label: DialNexa Phone Numbers API
  slug: dialnexa-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-phone-numbers-api-openapi.yml
- filename: dialnexa-transcribers-api-openapi.yml
  format: yaml
  label: DialNexa Transcribers API
  slug: dialnexa-transcribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-transcribers-api-openapi.yml
- filename: dialnexa-voices-api-openapi.yml
  format: yaml
  label: DialNexa Voices API
  slug: dialnexa-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-voices-api-openapi.yml
- filename: dialnexa-webhooks-api-openapi.yml
  format: yaml
  label: DialNexa Webhooks API
  slug: dialnexa-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-webhooks-api-openapi.yml
- filename: dialnexa-workflow-leads-api-openapi.yml
  format: yaml
  label: DialNexa Workflow Leads API
  slug: dialnexa-workflow-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-workflow-leads-api-openapi.yml
- filename: dialnexa-workflows-api-openapi.yml
  format: yaml
  label: DialNexa Workflows API
  slug: dialnexa-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/openapi/dialnexa-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dialnexa.com
  spf: true
hosts:
- cert_expires: Nov 24 06:43:13 2026 GMT
  host: dialnexa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 06:43:13 2026 GMT
  host: api.dialnexa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Dialnexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DialNexa, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DialNexa
provider_slug: dialnexa
slug: dialnexa-domain-security
source_filename: dialnexa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dialnexa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 06:43:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dialnexa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 06:43:13 2026 GMT\n  hsts: null\ndomains:\n- domain: dialnexa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialnexa/refs/heads/main/security/dialnexa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Voice AI
- AI Agents
- Telephony
- Lead Qualification
- Multilingual
---
