---
api_specs:
- filename: icallagent-public-api-agents-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Agents API
  slug: icallagent-public-api-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-agents-api-openapi.yml
- filename: icallagent-public-api-campaigns-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Campaigns API
  slug: icallagent-public-api-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-campaigns-api-openapi.yml
- filename: icallagent-public-api-contacts-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Contacts API
  slug: icallagent-public-api-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-contacts-api-openapi.yml
- filename: icallagent-public-api-phone-numbers-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Phone Numbers API
  slug: icallagent-public-api-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-phone-numbers-api-openapi.yml
- filename: icallagent-public-api-webhooks-api-openapi.yml
  format: yaml
  label: iCallAgent Public API Webhooks API
  slug: icallagent-public-api-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/openapi/icallagent-public-api-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: icallagent.com
  spf: true
hosts:
- cert_expires: Oct 28 20:44:18 2026 GMT
  host: docs.icallagent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 11:27:06 2026 GMT
  host: api.icallagent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Icallagent Public Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iCallAgent Public API, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: iCallAgent Public API
provider_slug: icallagent-public-api
slug: icallagent-public-api-domain-security
source_filename: icallagent-public-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.icallagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 20:44:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.icallagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 11:27:06 2026 GMT\n  hsts: null\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: icallagent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icallagent-public-api/refs/heads/main/security/icallagent-public-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice AI
- voice ai assistant
- Conversational AI
- Voice Agents
- telephony / CPaaS
- contact center / CCaaS
- Outbound Calling
- speech (ASR/TTS)
- agent tools / MCP
---
