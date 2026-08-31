---
api_specs:
- filename: anything-assets-api-openapi.yml
  format: yaml
  label: Anything Assets API
  slug: anything-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-assets-api-openapi.yml
- filename: anything-databases-api-openapi.yml
  format: yaml
  label: Anything Databases API
  slug: anything-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-databases-api-openapi.yml
- filename: anything-deployments-api-openapi.yml
  format: yaml
  label: Anything Deployments API
  slug: anything-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-deployments-api-openapi.yml
- filename: anything-domains-api-openapi.yml
  format: yaml
  label: Anything Domains API
  slug: anything-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-domains-api-openapi.yml
- filename: anything-files-api-openapi.yml
  format: yaml
  label: Anything Files API
  slug: anything-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-files-api-openapi.yml
- filename: anything-generation-api-openapi.yml
  format: yaml
  label: Anything Generation API
  slug: anything-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-generation-api-openapi.yml
- filename: anything-logs-api-openapi.yml
  format: yaml
  label: Anything Logs API
  slug: anything-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-logs-api-openapi.yml
- filename: anything-messages-api-openapi.yml
  format: yaml
  label: Anything Messages API
  slug: anything-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-messages-api-openapi.yml
- filename: anything-mobile-api-openapi.yml
  format: yaml
  label: Anything Mobile API
  slug: anything-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-mobile-api-openapi.yml
- filename: anything-organizations-api-openapi.yml
  format: yaml
  label: Anything Organizations API
  slug: anything-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-organizations-api-openapi.yml
- filename: anything-projects-api-openapi.yml
  format: yaml
  label: Anything Projects API
  slug: anything-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-projects-api-openapi.yml
- filename: anything-secrets-api-openapi.yml
  format: yaml
  label: Anything Secrets API
  slug: anything-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-secrets-api-openapi.yml
- filename: anything-settings-api-openapi.yml
  format: yaml
  label: Anything Settings API
  slug: anything-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-settings-api-openapi.yml
- filename: anything-user-api-openapi.yml
  format: yaml
  label: Anything User API
  slug: anything-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/openapi/anything-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: anything.com
  spf: true
hosts:
- cert_expires: Sep  9 22:35:07 2026 GMT
  host: www.anything.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anything Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anything, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Anything
provider_slug: anything
slug: anything-domain-security
source_filename: anything-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anything.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:35:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anything.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anything/refs/heads/main/security/anything-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai Ml
- App Builder
- Low Code
- No Code
- Developer Tools
- AI Agents
- Mobile
---
