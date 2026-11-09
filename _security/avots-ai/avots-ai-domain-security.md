---
api_specs:
- filename: app-avots-ai-openapi.json
  format: json
  label: OpenAI-compatible API
  slug: openai-compatible-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avots-ai/openapi/app-avots-ai-openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avots.ai
  spf: true
hosts:
- cert_expires: Dec 14 09:15:25 2026 GMT
  host: avots.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avots Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for avots.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: avots.ai
provider_slug: avots-ai
slug: avots-ai-domain-security
source_filename: avots-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avots.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 09:15:25 2026 GMT\n  hsts: false\ndomains:\n- domain: avots.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/avots-ai/security/avots-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Subscription
- Generative AI
- Platform
- Aggregator
---
