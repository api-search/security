---
api_specs:
- filename: alpic-analytics-api-openapi.yml
  format: yaml
  label: Alpic analytics API
  slug: alpic-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-analytics-api-openapi.yml
- filename: alpic-beacon-api-openapi.yml
  format: yaml
  label: Alpic beacon API
  slug: alpic-beacon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-beacon-api-openapi.yml
- filename: alpic-deployments-api-openapi.yml
  format: yaml
  label: Alpic deployments API
  slug: alpic-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-deployments-api-openapi.yml
- filename: alpic-distribution-api-openapi.yml
  format: yaml
  label: Alpic distribution API
  slug: alpic-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-distribution-api-openapi.yml
- filename: alpic-environments-api-openapi.yml
  format: yaml
  label: Alpic environments API
  slug: alpic-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-environments-api-openapi.yml
- filename: alpic-projects-api-openapi.yml
  format: yaml
  label: Alpic projects API
  slug: alpic-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-projects-api-openapi.yml
- filename: alpic-teams-api-openapi.yml
  format: yaml
  label: Alpic teams API
  slug: alpic-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-teams-api-openapi.yml
- filename: alpic-tunnels-api-openapi.yml
  format: yaml
  label: Alpic tunnels API
  slug: alpic-tunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-tunnels-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alpic.ai
  spf: true
hosts:
- cert_expires: Oct  4 10:57:23 2026 GMT
  host: alpic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.alpic.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alpic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alpic
provider_slug: alpic
slug: alpic-domain-security
source_filename: alpic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alpic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:57:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.alpic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: alpic.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/security/alpic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai/Ml
- MCP
- Cloud Platform
- Developer Tools
- Deployment
- ChatGPT Apps
- Agentic
---
