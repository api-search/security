---
api_specs:
- filename: rasa-domain-api-openapi.yml
  format: yaml
  label: Rasa Domain API
  slug: rasa-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-domain-api-openapi.yml
- filename: rasa-model-api-openapi.yml
  format: yaml
  label: Rasa Model API
  slug: rasa-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-model-api-openapi.yml
- filename: rasa-rasa-sdk-action-server-endpoint-api-openapi.yml
  format: yaml
  label: Rasa Rasa SDK Action Server Endpoint API
  slug: rasa-rasa-sdk-action-server-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-rasa-sdk-action-server-endpoint-api-openapi.yml
- filename: rasa-server-information-api-openapi.yml
  format: yaml
  label: Rasa Server Information API
  slug: rasa-server-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-server-information-api-openapi.yml
- filename: rasa-tracker-api-openapi.yml
  format: yaml
  label: Rasa Tracker API
  slug: rasa-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-tracker-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rasa.com
  spf: true
hosts:
- cert_expires: Sep 25 13:59:01 2026 GMT
  host: rasa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rasa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rasa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rasa
provider_slug: rasa
slug: rasa-domain-security
source_filename: rasa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rasa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:59:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rasa.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/security/rasa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Conversational AI
- Chatbots
- Voice Assistants
- NLU
- LLM
- Machine Learning
- Agents
---
