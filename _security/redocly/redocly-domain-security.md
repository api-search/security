---
api_specs:
- filename: redocly-health-api-openapi.yml
  format: yaml
  label: Redocly Health API
  slug: redocly-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-health-api-openapi.yml
- filename: redocly-metadata-api-openapi.yml
  format: yaml
  label: Redocly Metadata API
  slug: redocly-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-metadata-api-openapi.yml
- filename: redocly-remotes-api-openapi.yml
  format: yaml
  label: Redocly Remotes API
  slug: redocly-remotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-remotes-api-openapi.yml
- filename: redocly-search-api-openapi.yml
  format: yaml
  label: Redocly Search API
  slug: redocly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-search-api-openapi.yml
- filename: redocly-status-api-openapi.yml
  format: yaml
  label: Redocly Status API
  slug: redocly-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-status-api-openapi.yml
- filename: redocly-tasks-api-openapi.yml
  format: yaml
  label: Redocly Tasks API
  slug: redocly-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-tasks-api-openapi.yml
- filename: redocly-webhooks-api-openapi.yml
  format: yaml
  label: Redocly Webhooks API
  slug: redocly-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-webhooks-api-openapi.yml
- filename: redocly-to-dos-api-openapi.yml
  format: yaml
  label: Redocly To Dos API
  slug: redocly-to-dos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-to-dos-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: redocly.com
  spf: true
hosts:
- cert_expires: Oct  8 16:47:51 2026 GMT
  host: redocly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Redocly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redocly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Redocly
provider_slug: redocly
slug: redocly-domain-security
source_filename: redocly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redocly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:47:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: redocly.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/security/redocly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- API Catalog
- API Documentation
- Arazzo
- Developer Portal
- Governance
- Linting
- MCP
- Monitoring
- OpenAPI
---
