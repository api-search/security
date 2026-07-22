---
api_specs:
- filename: rasa-http-api-openapi.yml
  format: yaml
  label: Rasa HTTP API
  slug: rasa-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-http-api-openapi.yml
- filename: rasa-action-server-openapi.yml
  format: yaml
  label: Rasa SDK Action Server
  slug: rasa-sdk-action-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-action-server-openapi.yml
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
