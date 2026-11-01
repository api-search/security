---
api_specs:
- filename: airtop-profiles-api-openapi.yml
  format: yaml
  label: Airtop Profiles API
  slug: airtop-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-profiles-api-openapi.yml
- filename: airtop-sessions-api-openapi.yml
  format: yaml
  label: Airtop Sessions API
  slug: airtop-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-sessions-api-openapi.yml
- filename: airtop-windows-api-openapi.yml
  format: yaml
  label: Airtop Windows API
  slug: airtop-windows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-windows-api-openapi.yml
- filename: airtop-agent-director-api-openapi.yml
  format: yaml
  label: Airtop Agent Director API
  slug: airtop-agent-director-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-agent-director-api-openapi.yml
- filename: airtop-agent-folders-api-openapi.yml
  format: yaml
  label: Airtop Agent Folders API
  slug: airtop-agent-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-agent-folders-api-openapi.yml
- filename: airtop-agents-api-openapi.yml
  format: yaml
  label: Airtop Agents API
  slug: airtop-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-agents-api-openapi.yml
- filename: airtop-automations-api-openapi.yml
  format: yaml
  label: Airtop Automations API
  slug: airtop-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-automations-api-openapi.yml
- filename: airtop-beta-api-openapi.yml
  format: yaml
  label: Airtop Beta API
  slug: airtop-beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-beta-api-openapi.yml
- filename: airtop-files-api-openapi.yml
  format: yaml
  label: Airtop Files API
  slug: airtop-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-files-api-openapi.yml
- filename: airtop-gtm-engineer-api-openapi.yml
  format: yaml
  label: Airtop GTM Engineer API
  slug: airtop-gtm-engineer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-gtm-engineer-api-openapi.yml
- filename: airtop-knowledge-base-api-openapi.yml
  format: yaml
  label: Airtop Knowledge Base API
  slug: airtop-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-knowledge-base-api-openapi.yml
- filename: airtop-requests-api-openapi.yml
  format: yaml
  label: Airtop Requests API
  slug: airtop-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-requests-api-openapi.yml
- filename: airtop-sensitive-values-api-openapi.yml
  format: yaml
  label: Airtop Sensitive Values API
  slug: airtop-sensitive-values-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-sensitive-values-api-openapi.yml
- filename: airtop-services-api-openapi.yml
  format: yaml
  label: Airtop Services API
  slug: airtop-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-services-api-openapi.yml
- filename: airtop-team-vault-api-openapi.yml
  format: yaml
  label: Airtop Team Vault API
  slug: airtop-team-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-team-vault-api-openapi.yml
- filename: airtop-templates-api-openapi.yml
  format: yaml
  label: Airtop Templates API
  slug: airtop-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airtop.ai
  spf: true
hosts:
- cert_expires: Aug  9 20:52:19 2026 GMT
  host: www.airtop.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 16:12:13 2026 GMT
  host: docs.airtop.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.airtop.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Airtop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airtop, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airtop
provider_slug: airtop
slug: airtop-domain-security
source_filename: airtop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airtop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 20:52:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.airtop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:12:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.airtop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: airtop.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/airtop/security/airtop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser Automation
- AI Agents
- Cloud Browser
- Web Scraping
- Headless Chrome
---
