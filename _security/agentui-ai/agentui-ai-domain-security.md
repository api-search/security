---
api_specs:
- filename: agentui-ai-openapi-generated.yml
  format: yaml
  label: agentui-ai API
  slug: agentui-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentui-ai/openapi/_ae-authored/agentui-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentui.ai
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: agentui.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentui Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agentui-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: agentui-ai
provider_slug: agentui-ai
slug: agentui-ai-domain-security
source_filename: agentui-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentui.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: agentui.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentui-ai/security/agentui-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Internal-Tools
- Automation
- No-code
- LLM
- Company
---
