---
api_specs:
- filename: drift-com-accounts-api-openapi.yml
  format: yaml
  label: Drift Accounts API
  slug: drift-com-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-accounts-api-openapi.yml
- filename: drift-com-app-admin-api-openapi.yml
  format: yaml
  label: Drift App Admin API
  slug: drift-com-app-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-app-admin-api-openapi.yml
- filename: drift-com-contacts-api-openapi.yml
  format: yaml
  label: Drift Contacts API
  slug: drift-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-contacts-api-openapi.yml
- filename: drift-com-conversations-and-messages-api-openapi.yml
  format: yaml
  label: Drift Conversations and Messages API
  slug: drift-com-conversations-and-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-conversations-and-messages-api-openapi.yml
- filename: drift-com-data-privacy-api-openapi.yml
  format: yaml
  label: Drift Data Privacy API
  slug: drift-com-data-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-data-privacy-api-openapi.yml
- filename: drift-com-playbooks-api-openapi.yml
  format: yaml
  label: Drift Playbooks API
  slug: drift-com-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-playbooks-api-openapi.yml
- filename: drift-com-scim-api-api-openapi.yml
  format: yaml
  label: Drift SCIM API API
  slug: drift-com-scim-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-scim-api-api-openapi.yml
- filename: drift-com-teams-api-openapi.yml
  format: yaml
  label: Drift Teams API
  slug: drift-com-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-teams-api-openapi.yml
- filename: drift-com-users-api-openapi.yml
  format: yaml
  label: Drift Users API
  slug: drift-com-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/openapi/drift-com-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drift.com
  spf: true
hosts:
- cert_expires: Sep 26 20:17:29 2026 GMT
  host: www.drift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: app.drift.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:42:51 2026 GMT
  host: devdocs.drift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drift Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drift, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Drift
provider_slug: drift-com
slug: drift-com-domain-security
source_filename: drift-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:17:29 2026 GMT\n  hsts: false\n- host: app.drift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: devdocs.drift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:42:51 2026 GMT\n  hsts: null\ndomains:\n- domain: drift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drift-com/refs/heads/main/security/drift-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Conversational Marketing
- Chatbots
- Sales
- Messaging
- Customer Engagement
- Revenue Orchestration
- AI Chat
---
