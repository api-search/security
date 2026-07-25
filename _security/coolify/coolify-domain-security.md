---
api_specs:
- filename: coolify-applications-api-openapi.yml
  format: yaml
  label: Coolify Applications API
  slug: coolify-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-applications-api-openapi.yml
- filename: coolify-cloud-tokens-api-openapi.yml
  format: yaml
  label: Coolify Cloud Tokens API
  slug: coolify-cloud-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-cloud-tokens-api-openapi.yml
- filename: coolify-databases-api-openapi.yml
  format: yaml
  label: Coolify Databases API
  slug: coolify-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-databases-api-openapi.yml
- filename: coolify-deployments-api-openapi.yml
  format: yaml
  label: Coolify Deployments API
  slug: coolify-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-deployments-api-openapi.yml
- filename: coolify-disable-api-openapi.yml
  format: yaml
  label: Coolify Disable API
  slug: coolify-disable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-disable-api-openapi.yml
- filename: coolify-enable-api-openapi.yml
  format: yaml
  label: Coolify Enable API
  slug: coolify-enable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-enable-api-openapi.yml
- filename: coolify-github-apps-api-openapi.yml
  format: yaml
  label: Coolify GitHub Apps API
  slug: coolify-github-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-github-apps-api-openapi.yml
- filename: coolify-health-api-openapi.yml
  format: yaml
  label: Coolify Health API
  slug: coolify-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-health-api-openapi.yml
- filename: coolify-hetzner-api-openapi.yml
  format: yaml
  label: Coolify Hetzner API
  slug: coolify-hetzner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-hetzner-api-openapi.yml
- filename: coolify-mcp-api-openapi.yml
  format: yaml
  label: Coolify Mcp API
  slug: coolify-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-mcp-api-openapi.yml
- filename: coolify-private-keys-api-openapi.yml
  format: yaml
  label: Coolify Private Keys API
  slug: coolify-private-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-private-keys-api-openapi.yml
- filename: coolify-projects-api-openapi.yml
  format: yaml
  label: Coolify Projects API
  slug: coolify-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-projects-api-openapi.yml
- filename: coolify-resources-api-openapi.yml
  format: yaml
  label: Coolify Resources API
  slug: coolify-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-resources-api-openapi.yml
- filename: coolify-scheduled-tasks-api-openapi.yml
  format: yaml
  label: Coolify Scheduled Tasks API
  slug: coolify-scheduled-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-scheduled-tasks-api-openapi.yml
- filename: coolify-servers-api-openapi.yml
  format: yaml
  label: Coolify Servers API
  slug: coolify-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-servers-api-openapi.yml
- filename: coolify-services-api-openapi.yml
  format: yaml
  label: Coolify Services API
  slug: coolify-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-services-api-openapi.yml
- filename: coolify-teams-api-openapi.yml
  format: yaml
  label: Coolify Teams API
  slug: coolify-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-teams-api-openapi.yml
- filename: coolify-version-api-openapi.yml
  format: yaml
  label: Coolify Version API
  slug: coolify-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/openapi/coolify-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coolify.io
  spf: true
hosts:
- cert_expires: Aug 31 21:08:34 2026 GMT
  host: coolify.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 21:08:34 2026 GMT
  host: app.coolify.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coolify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coolify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coolify
provider_slug: coolify
slug: coolify-domain-security
source_filename: coolify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coolify.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:08:34 2026 GMT\n  hsts: false\n- host: app.coolify.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:08:34 2026 GMT\n  hsts: false\ndomains:\n- domain: coolify.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coolify/refs/heads/main/security/coolify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Platform as a Service
- Self-Hosting
- Deployment
- Open Source
- Containers
- Docker
---
