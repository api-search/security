---
api_specs:
- filename: n8n-audit-api-openapi.yml
  format: yaml
  label: N8n Audit API
  slug: n8n-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-audit-api-openapi.yml
- filename: n8n-communitypackage-api-openapi.yml
  format: yaml
  label: N8n CommunityPackage API
  slug: n8n-communitypackage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-communitypackage-api-openapi.yml
- filename: n8n-credential-api-openapi.yml
  format: yaml
  label: N8n Credential API
  slug: n8n-credential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-credential-api-openapi.yml
- filename: n8n-datatable-api-openapi.yml
  format: yaml
  label: N8n DataTable API
  slug: n8n-datatable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-datatable-api-openapi.yml
- filename: n8n-discover-api-openapi.yml
  format: yaml
  label: N8n Discover API
  slug: n8n-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-discover-api-openapi.yml
- filename: n8n-execution-api-openapi.yml
  format: yaml
  label: N8n Execution API
  slug: n8n-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-execution-api-openapi.yml
- filename: n8n-folders-api-openapi.yml
  format: yaml
  label: N8n Folders API
  slug: n8n-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-folders-api-openapi.yml
- filename: n8n-insights-api-openapi.yml
  format: yaml
  label: N8n Insights API
  slug: n8n-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-insights-api-openapi.yml
- filename: n8n-projects-api-openapi.yml
  format: yaml
  label: N8n Projects API
  slug: n8n-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-projects-api-openapi.yml
- filename: n8n-sourcecontrol-api-openapi.yml
  format: yaml
  label: N8n SourceControl API
  slug: n8n-sourcecontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-sourcecontrol-api-openapi.yml
- filename: n8n-tags-api-openapi.yml
  format: yaml
  label: N8n Tags API
  slug: n8n-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-tags-api-openapi.yml
- filename: n8n-user-api-openapi.yml
  format: yaml
  label: N8n User API
  slug: n8n-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-user-api-openapi.yml
- filename: n8n-variables-api-openapi.yml
  format: yaml
  label: N8n Variables API
  slug: n8n-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-variables-api-openapi.yml
- filename: n8n-workflow-api-openapi.yml
  format: yaml
  label: N8n Workflow API
  slug: n8n-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-workflow-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@n8n.io"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: n8n.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: n8n.cloud
  spf: true
hosts:
- cert_expires: Oct  3 02:40:24 2026 GMT
  host: n8n.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:12:10 2026 GMT
  host: docs.n8n.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 21:16:03 2026 GMT
  host: app.n8n.cloud
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: N8N Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for N8n, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: N8n
provider_slug: n8n
slug: n8n-domain-security
source_filename: n8n-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: n8n.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:40:24 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.n8n.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:12:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.n8n.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:16:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: n8n.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@n8n.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: n8n.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/security/n8n-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agents
- Artificial Intelligence
- Integration
---
