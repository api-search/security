---
api_specs:
- filename: unitary-ai-api-authentication-api-openapi.yml
  format: yaml
  label: Unitary AI API Authentication API
  slug: unitary-ai-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitary-ai/refs/heads/main/openapi/unitary-ai-api-authentication-api-openapi.yml
- filename: unitary-ai-detoxify-api-openapi.yml
  format: yaml
  label: Unitary AI Detoxify API
  slug: unitary-ai-detoxify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitary-ai/refs/heads/main/openapi/unitary-ai-detoxify-api-openapi.yml
- filename: unitary-ai-items-characteristics-api-openapi.yml
  format: yaml
  label: Unitary AI Items & Characteristics API
  slug: unitary-ai-items-characteristics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitary-ai/refs/heads/main/openapi/unitary-ai-items-characteristics-api-openapi.yml
- filename: unitary-ai-moderation-api-openapi.yml
  format: yaml
  label: Unitary AI moderation API
  slug: unitary-ai-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitary-ai/refs/heads/main/openapi/unitary-ai-moderation-api-openapi.yml
- filename: unitary-ai-policy-classification-api-openapi.yml
  format: yaml
  label: Unitary AI Policy Classification API
  slug: unitary-ai-policy-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitary-ai/refs/heads/main/openapi/unitary-ai-policy-classification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unitary.ai
  spf: true
hosts:
- cert_expires: Sep  9 07:14:52 2026 GMT
  host: www.unitary.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 22:01:19 2026 GMT
  host: docs.unitary.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:31:38 2026 GMT
  host: api.unitary.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unitary Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unitary AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unitary AI
provider_slug: unitary-ai
slug: unitary-ai-domain-security
source_filename: unitary-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unitary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:14:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.unitary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:01:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unitary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:31:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unitary.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitary-ai/refs/heads/main/security/unitary-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- Content Moderation
- Trust And Safety
- Artificial Intelligence
- Machine-Learning
- Computer-Vision
- Video
- Virtual Agents
---
