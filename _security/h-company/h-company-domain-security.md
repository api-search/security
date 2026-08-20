---
api_specs:
- filename: h-company-agents-api-openapi.yml
  format: yaml
  label: H Company Agents API
  slug: h-company-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-agents-api-openapi.yml
- filename: h-company-browser-profiles-api-openapi.yml
  format: yaml
  label: H Company Browser Profiles API
  slug: h-company-browser-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-browser-profiles-api-openapi.yml
- filename: h-company-environments-api-openapi.yml
  format: yaml
  label: H Company Environments API
  slug: h-company-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-environments-api-openapi.yml
- filename: h-company-quota-api-openapi.yml
  format: yaml
  label: H Company quota API
  slug: h-company-quota-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-quota-api-openapi.yml
- filename: h-company-schedules-api-openapi.yml
  format: yaml
  label: H Company Schedules API
  slug: h-company-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-schedules-api-openapi.yml
- filename: h-company-sessions-api-openapi.yml
  format: yaml
  label: H Company Sessions API
  slug: h-company-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-sessions-api-openapi.yml
- filename: h-company-skills-api-openapi.yml
  format: yaml
  label: H Company Skills API
  slug: h-company-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-skills-api-openapi.yml
- filename: h-company-vaults-api-openapi.yml
  format: yaml
  label: H Company Vaults API
  slug: h-company-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-vaults-api-openapi.yml
- filename: h-company-webhooks-api-openapi.yml
  format: yaml
  label: H Company Webhooks API
  slug: h-company-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hcompany.ai
  spf: true
hosts:
- cert_expires: Oct  4 10:34:48 2026 GMT
  host: www.hcompany.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: agp.eu.hcompany.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: agp.hcompany.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: H Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for H Company, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: H Company
provider_slug: h-company
slug: h-company-domain-security
source_filename: h-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hcompany.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 10:34:48 2026 GMT\n  hsts: null\n- host: agp.eu.hcompany.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\n- host: agp.hcompany.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hcompany.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/security/h-company-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Artificial Intelligence
- Agents
- Computer Use
- Automation
- Machine-Learning
- Browser Automation
- LLMs
- MCP
- Developer Tools
---
