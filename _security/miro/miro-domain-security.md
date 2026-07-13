---
api_specs:
- filename: miro-openapi.json
  format: json
  label: Miro Boards API
  slug: miro-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Board Items API
  slug: miro-board-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Connectors API
  slug: miro-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Tags API
  slug: miro-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Mind Map API
  slug: miro-mind-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Board Members API
  slug: miro-board-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Webhooks API
  slug: miro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Organization API
  slug: miro-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Teams API
  slug: miro-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Audit Logs API
  slug: miro-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro SCIM API
  slug: miro-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
- filename: miro-openapi.json
  format: json
  label: Miro Web SDK
  slug: miro-web-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/openapi/miro-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: miro.com
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: miro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 10:03:45 2026 GMT
  host: developers.miro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: api.miro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Miro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Miro
provider_slug: miro
slug: miro-domain-security
source_filename: miro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.miro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:03:45 2026 GMT\n  hsts: null\n- host: api.miro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: miro.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miro/refs/heads/main/security/miro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Productivity
- Whiteboard
- Visual Collaboration
- Diagramming
- SaaS
---
