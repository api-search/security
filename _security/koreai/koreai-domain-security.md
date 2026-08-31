---
api_specs:
- filename: Public-APIs
  format: yaml
  label: Kore.ai AI for Service Platform APIs
  slug: koreai-ai-for-service-platform-apis
  spec_type: Postman
  url: https://github.com/Koredotcom/Public-APIs
- filename: koreai-chat-api-openapi.yml
  format: yaml
  label: Kore.ai Chat API
  slug: koreai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-chat-api-openapi.yml
- filename: koreai-conversation-api-openapi.yml
  format: yaml
  label: Kore.ai Conversation API
  slug: koreai-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-conversation-api-openapi.yml
- filename: koreai-workflows-api-openapi.yml
  format: yaml
  label: Kore.ai Workflows API
  slug: koreai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/openapi/koreai-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kore.ai
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.kore.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.kore.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: agents.kore.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koreai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kore.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kore.ai
provider_slug: koreai
slug: koreai-domain-security
source_filename: koreai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: agents.kore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kore.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koreai/refs/heads/main/security/koreai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Agents
- Agent Platform
- Contact Center
- Customer Experience
- Employee Experience
- Voice
- Automation
- Model Context Protocol
- Enterprise Software
---
