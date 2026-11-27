---
api_specs:
- filename: mentionagent-ai-authority-api-openapi.yml
  format: yaml
  label: MentionAgent Authority API
  slug: mentionagent-ai-authority-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionagent-ai/openapi/mentionagent-ai-authority-api-openapi.yml
- filename: mentionagent-ai-site-api-openapi.yml
  format: yaml
  label: MentionAgent Site API
  slug: mentionagent-ai-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentionagent-ai/openapi/mentionagent-ai-site-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mentionagent.ai
  spf: false
hosts:
- cert_expires: Jan 20 06:48:22 2027 GMT
  host: mentionagent.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MentionAgent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MentionAgent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MentionAgent
provider_slug: mentionagent-ai
slug: mentionagent-ai-domain-security
source_filename: mentionagent-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mentionagent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 06:48:22 2027 GMT\n  hsts: false\ndomains:\n- domain: mentionagent.ai\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mentionagent-ai/security/mentionagent-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SEO
- Artificial Intelligence
- Link Building
- Marketing
- Software-as-a-Service
---
