---
api_specs:
- filename: cirra-ai-openapi-generated.yml
  format: yaml
  label: Cirra AI API
  slug: cirra-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cirra-ai/openapi/_ae-authored/cirra-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@cirra.ai"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cirra.ai
  spf: true
hosts:
- cert_expires: Jan  2 09:35:04 2027 GMT
  host: cirra.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cirra Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cirra AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cirra AI
provider_slug: cirra-ai
slug: cirra-ai-domain-security
source_filename: cirra-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cirra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 09:35:04 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cirra.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@cirra.ai\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cirra-ai/security/cirra-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Salesforce
- MCP
- Admin
- Software-as-a-Service
---
