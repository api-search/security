---
api_specs:
- filename: smartlead-ai-campaign-statistics-api-openapi.yml
  format: yaml
  label: Smartlead Campaign Statistics API
  slug: smartlead-ai-campaign-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-campaign-statistics-api-openapi.yml
- filename: smartlead-ai-campaigns-api-openapi.yml
  format: yaml
  label: Smartlead Campaigns API
  slug: smartlead-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-campaigns-api-openapi.yml
- filename: smartlead-ai-analytics-api-openapi.yml
  format: yaml
  label: Smartlead Analytics API
  slug: smartlead-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-analytics-api-openapi.yml
- filename: smartlead-ai-authentication-api-openapi.yml
  format: yaml
  label: Smartlead Authentication API
  slug: smartlead-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-authentication-api-openapi.yml
- filename: smartlead-ai-email-accounts-api-openapi.yml
  format: yaml
  label: Smartlead Email Accounts API
  slug: smartlead-ai-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-email-accounts-api-openapi.yml
- filename: smartlead-ai-leads-api-openapi.yml
  format: yaml
  label: Smartlead Leads API
  slug: smartlead-ai-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-leads-api-openapi.yml
- filename: smartlead-ai-master-inbox-api-openapi.yml
  format: yaml
  label: Smartlead Master Inbox API
  slug: smartlead-ai-master-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-master-inbox-api-openapi.yml
- filename: smartlead-ai-smart-delivery-api-openapi.yml
  format: yaml
  label: Smartlead Smart Delivery API
  slug: smartlead-ai-smart-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-smart-delivery-api-openapi.yml
- filename: smartlead-ai-smart-senders-api-openapi.yml
  format: yaml
  label: Smartlead Smart Senders API
  slug: smartlead-ai-smart-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-smart-senders-api-openapi.yml
- filename: smartlead-ai-utilities-api-openapi.yml
  format: yaml
  label: Smartlead Utilities API
  slug: smartlead-ai-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-utilities-api-openapi.yml
- filename: smartlead-ai-webhooks-api-openapi.yml
  format: yaml
  label: Smartlead Webhooks API
  slug: smartlead-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/openapi/smartlead-ai-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smartlead.ai
  spf: true
hosts:
- cert_expires: Sep 29 16:23:28 2026 GMT
  host: www.smartlead.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 17:18:16 2026 GMT
  host: api.smartlead.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:04:39 2026 GMT
  host: server.smartlead.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartlead Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartlead, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Smartlead
provider_slug: smartlead-ai
slug: smartlead-ai-domain-security
source_filename: smartlead-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartlead.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:23:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smartlead.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:18:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: server.smartlead.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:04:39 2026 GMT\n  hsts: null\ndomains:\n- domain: smartlead.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartlead-ai/refs/heads/main/security/smartlead-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cold Email
- Outbound
- Sales
- Deliverability
- Email Warm-up
- Automation
- Sequences
---
