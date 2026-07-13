---
api_specs:
- filename: phonely-agents-api-openapi.yml
  format: yaml
  label: Phonely Agents API
  slug: phonely-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/openapi/phonely-agents-api-openapi.yml
- filename: phonely-webhooks-asyncapi.yml
  format: yaml
  label: Phonely Webhooks API
  slug: phonely-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/asyncapi/phonely-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: phonely.ai
  spf: true
hosts:
- cert_expires: Aug 23 23:29:18 2026 GMT
  host: www.phonely.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:38:32 2026 GMT
  host: docs.phonely.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:38:32 2026 GMT
  host: app.phonely.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phonely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phonely, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Phonely
provider_slug: phonely
slug: phonely-domain-security
source_filename: phonely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phonely.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:29:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.phonely.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:38:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.phonely.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:38:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: phonely.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phonely/refs/heads/main/security/phonely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- Voice AI
- Voice Agents
- Conversational AI
- Telephony
- Phone
- Call Center
- Contact Center
- SMS
- Webhooks
- Workflow Automation
- Scheduling
- CRM
---
