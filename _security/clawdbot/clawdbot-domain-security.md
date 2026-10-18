---
api_specs:
- filename: clawdbot-clawdbot-api-api-openapi.yml
  format: yaml
  label: Clawdbot Clawdbot API
  slug: clawdbot-clawdbot-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdbot/refs/heads/main/openapi/clawdbot-clawdbot-api-api-openapi.yml
- filename: clawdbot-npm-api-openapi.yml
  format: yaml
  label: Clawdbot Npm API
  slug: clawdbot-npm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdbot/refs/heads/main/openapi/clawdbot-npm-api-openapi.yml
- filename: clawdbot-packages-api-openapi.yml
  format: yaml
  label: Clawdbot Packages API
  slug: clawdbot-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdbot/refs/heads/main/openapi/clawdbot-packages-api-openapi.yml
- filename: clawdbot-plugins-api-openapi.yml
  format: yaml
  label: Clawdbot Plugins API
  slug: clawdbot-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdbot/refs/heads/main/openapi/clawdbot-plugins-api-openapi.yml
- filename: clawdbot-skills-api-openapi.yml
  format: yaml
  label: Clawdbot Skills API
  slug: clawdbot-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdbot/refs/heads/main/openapi/clawdbot-skills-api-openapi.yml
- filename: clawdbot-transfers-api-openapi.yml
  format: yaml
  label: Clawdbot Transfers API
  slug: clawdbot-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdbot/refs/heads/main/openapi/clawdbot-transfers-api-openapi.yml
- filename: clawdbot-users-api-openapi.yml
  format: yaml
  label: Clawdbot Users API
  slug: clawdbot-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawdbot/refs/heads/main/openapi/clawdbot-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openclaw.ai
  spf: true
hosts:
- cert_expires: Jan  6 03:51:06 2027 GMT
  host: openclaw.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clawdbot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clawdbot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Clawdbot
provider_slug: clawdbot
slug: clawdbot-domain-security
source_filename: clawdbot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openclaw.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 03:51:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openclaw.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clawdbot/refs/heads/main/security/clawdbot-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Open Source
- PersonalAssistant
- Automation
---
