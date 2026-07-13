---
api_specs:
- filename: openapi.json
  format: json
  label: Microsoft Copilot API
  slug: microsoft-copilot-api
  spec_type: OpenAPI
  url: https://api.copilot.microsoft.com/openapi.json
- filename: openapi.json
  format: json
  label: Microsoft Graph API (Copilot Integration)
  slug: microsoft-graph-api-copilot-integration
  spec_type: OpenAPI
  url: https://graph.microsoft.com/openapi.json
- filename: microsoft-copilot-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot APIs
  slug: microsoft-365-copilot-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/openapi/microsoft-copilot-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 20 02:11:36 2026 GMT
  host: developer.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.copilot.microsoft.com
  https: false
kind: domain-security
layout: security
method: probed
name: Microsoft Copilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Copilot, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
slug: microsoft-copilot-domain-security
source_filename: microsoft-copilot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.copilot.microsoft.com\n  https: false\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/security/microsoft-copilot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft 365
- Productivity
---
