---
api_specs:
- filename: preset-openapi.yml
  format: yaml
  label: Preset Auth API
  slug: preset-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Teams and Workspaces API
  slug: preset-teams-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Dashboards API
  slug: preset-superset-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Charts API
  slug: preset-superset-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Datasets API
  slug: preset-superset-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset Databases API
  slug: preset-superset-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
- filename: preset-openapi.yml
  format: yaml
  label: Preset Superset SQL Lab API
  slug: preset-superset-sqllab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/openapi/preset-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@preset.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: preset.io
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.preset.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 23:44:16 2026 GMT
  host: api-docs.preset.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.app.preset.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Preset Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preset, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Preset
provider_slug: preset
slug: preset-domain-security
source_filename: preset-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.preset.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.preset.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:44:16 2026 GMT\n  hsts: null\n- host: api.app.preset.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: preset.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@preset.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preset/refs/heads/main/security/preset-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BI
- Analytics
- Superset
- Dashboards
- Data Visualization
---
