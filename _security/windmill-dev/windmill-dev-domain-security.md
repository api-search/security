---
api_specs:
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Scripts API
  slug: windmill-dev-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Flows API
  slug: windmill-dev-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Apps API
  slug: windmill-dev-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Jobs API
  slug: windmill-dev-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Schedules API
  slug: windmill-dev-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Variables API
  slug: windmill-dev-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Resources API
  slug: windmill-dev-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Workspaces API
  slug: windmill-dev-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Users API
  slug: windmill-dev-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Groups API
  slug: windmill-dev-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Folders API
  slug: windmill-dev-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Audit Logs API
  slug: windmill-dev-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Workers API
  slug: windmill-dev-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Triggers API
  slug: windmill-dev-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill OIDC API
  slug: windmill-dev-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: windmill.dev
  spf: true
hosts:
- cert_expires: Oct  2 05:54:27 2026 GMT
  host: www.windmill.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: app.windmill.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Windmill Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Windmill, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Windmill
provider_slug: windmill-dev
slug: windmill-dev-domain-security
source_filename: windmill-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.windmill.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:54:27 2026 GMT\n  hsts: false\n- host: app.windmill.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: windmill.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/security/windmill-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Developer Platform
- Workflows
- Internal Tools
- Job Orchestration
- Cron
- Open Source
---
