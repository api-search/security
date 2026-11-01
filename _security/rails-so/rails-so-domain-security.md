---
api_specs:
- filename: rails-so-api-openapi.json
  format: json
  label: Agent Rails public MCP and OAuth HTTP API API
  slug: agent-rails-public-mcp-and-oauth-http-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rails-so/openapi/_original/rails-so-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rails.so
  spf: true
hosts:
- cert_expires: Dec 18 04:11:36 2026 GMT
  host: rails.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rails So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rails-so, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: rails-so
provider_slug: rails-so
slug: rails-so-domain-security
source_filename: rails-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rails.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 04:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rails.so\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rails-so/security/rails-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Automation
- Productivity
- Collaboration
- ChatGPT
- Claude
- Company
---
