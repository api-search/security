---
api_specs:
- filename: render-com-openapi.yml
  format: yaml
  label: Render Services API
  slug: render-com-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Deploys API
  slug: render-com-deploys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Custom Domains API
  slug: render-com-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Environment Variables & Secret Files API
  slug: render-com-env-vars-secret-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Environment Groups API
  slug: render-com-env-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Postgres API
  slug: render-com-postgres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Key Value API
  slug: render-com-key-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Jobs API
  slug: render-com-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Disks API
  slug: render-com-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Blueprints API
  slug: render-com-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Projects & Environments API
  slug: render-com-projects-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Workspaces & Members API
  slug: render-com-workspaces-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Metrics API
  slug: render-com-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Logs API
  slug: render-com-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
- filename: render-com-openapi.yml
  format: yaml
  label: Render Webhooks API
  slug: render-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/openapi/render-com-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@render.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: render.com
  spf: true
hosts:
- cert_expires: Aug 21 19:26:00 2026 GMT
  host: render.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 07:36:18 2026 GMT
  host: api-docs.render.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 01:57:23 2026 GMT
  host: api.render.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Render Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Render, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Render
provider_slug: render-com
slug: render-com-domain-security
source_filename: render-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: render.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:26:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.render.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:36:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.render.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:57:23 2026 GMT\n  hsts: null\ndomains:\n- domain: render.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@render.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/render-com/refs/heads/main/security/render-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Hosting
- PaaS
- Deployment
- Web Services
- Databases
- DevOps
---
