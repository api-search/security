---
api_specs:
- filename: fixie-accounts-api-openapi.yml
  format: yaml
  label: Fixie Accounts API
  slug: fixie-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-accounts-api-openapi.yml
- filename: fixie-agents-api-openapi.yml
  format: yaml
  label: Fixie Agents API
  slug: fixie-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-agents-api-openapi.yml
- filename: fixie-api-keys-api-openapi.yml
  format: yaml
  label: Fixie API Keys API
  slug: fixie-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-api-keys-api-openapi.yml
- filename: fixie-call-throttles-api-openapi.yml
  format: yaml
  label: Fixie Call Throttles API
  slug: fixie-call-throttles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-call-throttles-api-openapi.yml
- filename: fixie-calls-api-openapi.yml
  format: yaml
  label: Fixie Calls API
  slug: fixie-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-calls-api-openapi.yml
- filename: fixie-corpora-api-openapi.yml
  format: yaml
  label: Fixie Corpora API
  slug: fixie-corpora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-corpora-api-openapi.yml
- filename: fixie-deleted-calls-api-openapi.yml
  format: yaml
  label: Fixie Deleted Calls API
  slug: fixie-deleted-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-deleted-calls-api-openapi.yml
- filename: fixie-models-api-openapi.yml
  format: yaml
  label: Fixie Models API
  slug: fixie-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-models-api-openapi.yml
- filename: fixie-schema-api-openapi.yml
  format: yaml
  label: Fixie Schema API
  slug: fixie-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-schema-api-openapi.yml
- filename: fixie-sip-api-openapi.yml
  format: yaml
  label: Fixie Sip API
  slug: fixie-sip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-sip-api-openapi.yml
- filename: fixie-telephony-configs-api-openapi.yml
  format: yaml
  label: Fixie Telephony Configs API
  slug: fixie-telephony-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-telephony-configs-api-openapi.yml
- filename: fixie-tools-api-openapi.yml
  format: yaml
  label: Fixie Tools API
  slug: fixie-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-tools-api-openapi.yml
- filename: fixie-voices-api-openapi.yml
  format: yaml
  label: Fixie Voices API
  slug: fixie-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-voices-api-openapi.yml
- filename: fixie-webhooks-api-openapi.yml
  format: yaml
  label: Fixie Webhooks API
  slug: fixie-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/openapi/fixie-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fixie.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ultravox.ai
  spf: true
hosts:
- cert_expires: Sep 23 09:41:45 2026 GMT
  host: www.fixie.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 07:04:09 2026 GMT
  host: api.ultravox.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Fixie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixie, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fixie
provider_slug: fixie
slug: fixie-domain-security
source_filename: fixie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fixie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:41:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ultravox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:04:09 2026 GMT\n  hsts: false\ndomains:\n- domain: fixie.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ultravox.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixie/refs/heads/main/security/fixie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Voice AI
- Conversational AI
- Real-Time
- Speech
- Agents
- Telephony
- Machine Learning
- SIP
- Webhook
---
