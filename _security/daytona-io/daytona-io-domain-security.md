---
api_specs:
- filename: daytona-sandbox-api-openapi.yml
  format: yaml
  label: Daytona Sandbox API
  slug: daytona-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-sandbox-api-openapi.yml
- filename: daytona-sandbox-toolbox-api-openapi.yml
  format: yaml
  label: Daytona Sandbox Toolbox API
  slug: daytona-sandbox-toolbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-sandbox-toolbox-api-openapi.yml
- filename: daytona-snapshots-api-openapi.yml
  format: yaml
  label: Daytona Snapshots API
  slug: daytona-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-snapshots-api-openapi.yml
- filename: daytona-volumes-api-openapi.yml
  format: yaml
  label: Daytona Volumes API
  slug: daytona-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-volumes-api-openapi.yml
- filename: daytona-preview-api-openapi.yml
  format: yaml
  label: Daytona Preview API
  slug: daytona-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-preview-api-openapi.yml
- filename: daytona-webhooks-api-openapi.yml
  format: yaml
  label: Daytona Webhooks API
  slug: daytona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-webhooks-api-openapi.yml
- filename: daytona-organizations-api-openapi.yml
  format: yaml
  label: Daytona Organizations API
  slug: daytona-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-organizations-api-openapi.yml
- filename: daytona-api-keys-api-openapi.yml
  format: yaml
  label: Daytona API Keys API
  slug: daytona-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-api-keys-api-openapi.yml
- filename: daytona-users-api-openapi.yml
  format: yaml
  label: Daytona Users API
  slug: daytona-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-users-api-openapi.yml
- filename: daytona-admin-api-openapi.yml
  format: yaml
  label: Daytona Admin API
  slug: daytona-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-admin-api-openapi.yml
- filename: daytona-health-api-openapi.yml
  format: yaml
  label: Daytona Health API
  slug: daytona-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/openapi/daytona-health-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@daytona.io"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: daytona.io
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.daytona.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: app.daytona.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: proxy.app.daytona.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daytona Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daytona, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Daytona
provider_slug: daytona-io
slug: daytona-io-domain-security
source_filename: daytona-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.daytona.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.daytona.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: proxy.app.daytona.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: daytona.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@daytona.io\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daytona-io/refs/heads/main/security/daytona-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Agents
- Artificial Intelligence
- Cloud
- Code Execution
- Computer Use
- Developer Tools
- Infrastructure
- Open Source
- Sandbox
- Secure Execution
---
