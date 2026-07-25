---
api_specs:
- filename: postman-webhooks-asyncapi.yml
  format: yaml
  label: Postman
  slug: postman
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/asyncapi/postman-webhooks-asyncapi.yml
- filename: postman-collections-api-openapi.yml
  format: yaml
  label: Postman Collections API
  slug: collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-collections-api-openapi.yml
- filename: postman-workspaces-api-openapi.yml
  format: yaml
  label: Postman Workspaces API
  slug: workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-workspaces-api-openapi.yml
- filename: postman-environments-api-openapi.yml
  format: yaml
  label: Postman Environments API
  slug: environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-environments-api-openapi.yml
- filename: postman-monitors-api-openapi.yml
  format: yaml
  label: Postman Monitors API
  slug: monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-monitors-api-openapi.yml
- filename: postman-apis-api-openapi.yml
  format: yaml
  label: Postman APIs / Spec Hub API
  slug: apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-apis-api-openapi.yml
- filename: postman-private-api-network-api-openapi.yml
  format: yaml
  label: Postman Private API Network API
  slug: private-api-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-private-api-network-api-openapi.yml
- filename: postman-webhooks-api-openapi.yml
  format: yaml
  label: Postman Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-webhooks-api-openapi.yml
- filename: postman-collection-runs-api-openapi.yml
  format: yaml
  label: Postman Collection Runs API
  slug: collection-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-collection-runs-api-openapi.yml
- filename: postman-tags-api-openapi.yml
  format: yaml
  label: Postman Tags API
  slug: tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-tags-api-openapi.yml
- filename: postman-audit-logs-api-openapi.yml
  format: yaml
  label: Postman Audit Logs API
  slug: audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-audit-logs-api-openapi.yml
- filename: postman-secret-scanner-api-openapi.yml
  format: yaml
  label: Postman Secret Scanner API
  slug: secret-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-secret-scanner-api-openapi.yml
- filename: postman-api-comments-api-openapi.yml
  format: yaml
  label: Postman API Comments API
  slug: postman-api-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-api-comments-api-openapi.yml
- filename: postman-api-schemas-api-openapi.yml
  format: yaml
  label: Postman API Schemas API
  slug: postman-api-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-api-schemas-api-openapi.yml
- filename: postman-api-versions-api-openapi.yml
  format: yaml
  label: Postman API Versions API
  slug: postman-api-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-api-versions-api-openapi.yml
- filename: postman-mocks-api-openapi.yml
  format: yaml
  label: Postman Mocks API
  slug: postman-mocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-mocks-api-openapi.yml
- filename: postman-network-elements-api-openapi.yml
  format: yaml
  label: Postman Network Elements API
  slug: postman-network-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-network-elements-api-openapi.yml
- filename: postman-network-folders-api-openapi.yml
  format: yaml
  label: Postman Network Folders API
  slug: postman-network-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-network-folders-api-openapi.yml
- filename: postman-network-requests-api-openapi.yml
  format: yaml
  label: Postman Network Requests API
  slug: postman-network-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-network-requests-api-openapi.yml
- filename: postman-server-responses-api-openapi.yml
  format: yaml
  label: Postman Server Responses API
  slug: postman-server-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-server-responses-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postman.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpostman.com
  spf: true
hosts:
- cert_expires: Aug 16 09:00:12 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:02:05 2026 GMT
  host: api.getpostman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:17:28 2026 GMT
  host: learning.postman.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postman, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Postman
provider_slug: postman
slug: postman-domain-security
source_filename: postman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getpostman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learning.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:17:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: postman.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getpostman.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0\
  \ issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/security/postman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agent Builder
- AI Agents
- API Catalog
- API Client
- API Design
- API Development
- API Documentation
- API Governance
- API Lifecycle
- API Monitoring
- API Network
- API Platform
- API Testing
- Audit Logs
- Automation
- CI/CD
- Collaboration
- Collections
- Compliance
- Discovery
- Environments
- Flows
- GraphQL
- gRPC
- HTTP
- Insights
- MCP
- MCP Generator
- Mock Servers
- Mocking
- Monitors
- Newman
- OpenAPI
- Platform
- Private API Network
- Public API Network
- Secret Scanning
- Spec Hub
- Specifications
- SSO
- Testing
- Vault
- WebSocket
- Workflows
- Workspaces
---
