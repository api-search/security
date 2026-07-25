---
api_specs:
- filename: capy-automations-api-openapi.yml
  format: yaml
  label: Capy automations API
  slug: capy-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-automations-api-openapi.yml
- filename: capy-browser-snapshots-api-openapi.yml
  format: yaml
  label: Capy browser-snapshots API
  slug: capy-browser-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-browser-snapshots-api-openapi.yml
- filename: capy-environment-variables-api-openapi.yml
  format: yaml
  label: Capy environment-variables API
  slug: capy-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-environment-variables-api-openapi.yml
- filename: capy-models-api-openapi.yml
  format: yaml
  label: Capy models API
  slug: capy-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-models-api-openapi.yml
- filename: capy-projects-api-openapi.yml
  format: yaml
  label: Capy projects API
  slug: capy-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-projects-api-openapi.yml
- filename: capy-sessions-api-openapi.yml
  format: yaml
  label: Capy sessions API
  slug: capy-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-sessions-api-openapi.yml
- filename: capy-setup-api-openapi.yml
  format: yaml
  label: Capy setup API
  slug: capy-setup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-setup-api-openapi.yml
- filename: capy-snapshots-api-openapi.yml
  format: yaml
  label: Capy snapshots API
  slug: capy-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-snapshots-api-openapi.yml
- filename: capy-tags-api-openapi.yml
  format: yaml
  label: Capy tags API
  slug: capy-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-tags-api-openapi.yml
- filename: capy-tasks-api-openapi.yml
  format: yaml
  label: Capy tasks API
  slug: capy-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-tasks-api-openapi.yml
- filename: capy-threads-api-openapi.yml
  format: yaml
  label: Capy threads API
  slug: capy-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-threads-api-openapi.yml
- filename: capy-usage-api-openapi.yml
  format: yaml
  label: Capy usage API
  slug: capy-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-usage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: capy.ai
  spf: true
hosts:
- cert_expires: Oct  4 08:19:27 2026 GMT
  host: capy.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Capy
provider_slug: capy
slug: capy-domain-security
source_filename: capy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:19:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capy.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/security/capy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- AI Coding Agent
- Software Engineering
- Developer Tools
- Automation
- Code Review
- DevOps
---
