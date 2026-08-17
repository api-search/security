---
api_specs:
- filename: apollo-api-documentation-accounts-api-openapi.yml
  format: yaml
  label: Apollo API Accounts
  slug: apollo-api-documentation-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-accounts-api-openapi.yml
- filename: apollo-api-documentation-analytics-api-openapi.yml
  format: yaml
  label: Apollo API Analytics
  slug: apollo-api-documentation-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-analytics-api-openapi.yml
- filename: apollo-api-documentation-calls-api-openapi.yml
  format: yaml
  label: Apollo API Calls
  slug: apollo-api-documentation-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-calls-api-openapi.yml
- filename: apollo-api-documentation-contacts-api-openapi.yml
  format: yaml
  label: Apollo API Contacts
  slug: apollo-api-documentation-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-contacts-api-openapi.yml
- filename: apollo-api-documentation-conversations-api-openapi.yml
  format: yaml
  label: Apollo API Conversations
  slug: apollo-api-documentation-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-conversations-api-openapi.yml
- filename: apollo-api-documentation-deals-api-openapi.yml
  format: yaml
  label: Apollo API Deals
  slug: apollo-api-documentation-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-deals-api-openapi.yml
- filename: apollo-api-documentation-emailer-messages-api-openapi.yml
  format: yaml
  label: Apollo API Emailer Messages
  slug: apollo-api-documentation-emailer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-emailer-messages-api-openapi.yml
- filename: apollo-api-documentation-enrichment-api-openapi.yml
  format: yaml
  label: Apollo API Enrichment
  slug: apollo-api-documentation-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-enrichment-api-openapi.yml
- filename: apollo-api-documentation-fields-api-openapi.yml
  format: yaml
  label: Apollo API Fields
  slug: apollo-api-documentation-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-fields-api-openapi.yml
- filename: apollo-api-documentation-miscellaneous-api-openapi.yml
  format: yaml
  label: Apollo API Miscellaneous
  slug: apollo-api-documentation-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-miscellaneous-api-openapi.yml
- filename: apollo-api-documentation-search-api-openapi.yml
  format: yaml
  label: Apollo API Search
  slug: apollo-api-documentation-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-search-api-openapi.yml
- filename: apollo-api-documentation-sequences-api-openapi.yml
  format: yaml
  label: Apollo API Sequences
  slug: apollo-api-documentation-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-sequences-api-openapi.yml
- filename: apollo-api-documentation-tasks-api-openapi.yml
  format: yaml
  label: Apollo API Tasks
  slug: apollo-api-documentation-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-tasks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apollo.io
  spf: true
hosts:
- cert_expires: Oct  3 09:31:14 2026 GMT
  host: docs.apollo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 12:24:25 2026 GMT
  host: api.apollo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 12:24:25 2026 GMT
  host: mcp.apollo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apollo Api Documentation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo API Documentation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apollo API Documentation
provider_slug: apollo-api-documentation
slug: apollo-api-documentation-domain-security
source_filename: apollo-api-documentation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 12:24:25 2026 GMT\n  hsts: null\n- host: mcp.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 12:24:25 2026 GMT\n  hsts: null\ndomains:\n- domain: apollo.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/security/apollo-api-documentation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Documentation
- Sales Intelligence
- Data Enrichment
- People Search
- Company Search
- Sales Engagement
- CRM
- MCP
- Agents
- Go-To-Market
---
