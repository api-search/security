---
api_specs:
- filename: capy-automations-api-openapi.yml
  format: yaml
  label: Capy Automations API
  slug: capy-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-automations-api-openapi.yml
- filename: capy-projects-api-openapi.yml
  format: yaml
  label: Capy Projects API
  slug: capy-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-projects-api-openapi.yml
- filename: capy-tasks-api-openapi.yml
  format: yaml
  label: Capy Tasks API
  slug: capy-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-tasks-api-openapi.yml
- filename: capy-threads-api-openapi.yml
  format: yaml
  label: Capy Threads API
  slug: capy-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-threads-api-openapi.yml
- filename: capy-usage-api-openapi.yml
  format: yaml
  label: Capy Usage API
  slug: capy-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-usage-api-openapi.yml
- filename: capy-captains-api-openapi.yml
  format: yaml
  label: Capy Captains API
  slug: capy-captains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-captains-api-openapi.yml
- filename: capy-folders-api-openapi.yml
  format: yaml
  label: Capy Folders API
  slug: capy-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-folders-api-openapi.yml
- filename: capy-messages-api-openapi.yml
  format: yaml
  label: Capy Messages API
  slug: capy-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-messages-api-openapi.yml
- filename: capy-reviewfilters-api-openapi.yml
  format: yaml
  label: Capy Review Filters API
  slug: capy-reviewfilters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-reviewfilters-api-openapi.yml
- filename: capy-reviewrules-api-openapi.yml
  format: yaml
  label: Capy Review Rules API
  slug: capy-reviewrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-reviewrules-api-openapi.yml
- filename: capy-reviews-api-openapi.yml
  format: yaml
  label: Capy Reviews API
  slug: capy-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-reviews-api-openapi.yml
- filename: capy-streams-api-openapi.yml
  format: yaml
  label: Capy Streams API
  slug: capy-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-streams-api-openapi.yml
- filename: capy-subagents-api-openapi.yml
  format: yaml
  label: Capy Subagents API
  slug: capy-subagents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-subagents-api-openapi.yml
- filename: capy-users-api-openapi.yml
  format: yaml
  label: Capy Users API
  slug: capy-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capy/openapi/capy-users-api-openapi.yml
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
hosts_probed: 1
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
source_yaml_url: https://artifacts.apis.io/capy/security/capy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Coding Agents
- Software Engineering
- Developer Tools
- Automation
- Code Review
- DevOps
---
