---
api_specs:
- filename: apollo-io-enrichment-api-openapi.yml
  format: yaml
  label: Apollo.io Enrichment API
  slug: apollo-io-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-enrichment-api-openapi.yml
- filename: apollo-io-search-api-openapi.yml
  format: yaml
  label: Apollo.io Search API
  slug: apollo-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-search-api-openapi.yml
- filename: apollo-io-accounts-api-openapi.yml
  format: yaml
  label: Apollo.io Accounts API
  slug: apollo-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-accounts-api-openapi.yml
- filename: apollo-io-contacts-api-openapi.yml
  format: yaml
  label: Apollo.io Contacts API
  slug: apollo-io-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-contacts-api-openapi.yml
- filename: apollo-io-deals-api-openapi.yml
  format: yaml
  label: Apollo.io Deals API
  slug: apollo-io-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-deals-api-openapi.yml
- filename: apollo-io-sequences-api-openapi.yml
  format: yaml
  label: Apollo.io Sequences API
  slug: apollo-io-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-sequences-api-openapi.yml
- filename: apollo-io-emailer-messages-api-openapi.yml
  format: yaml
  label: Apollo.io Emailer Messages API
  slug: apollo-io-emailer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-emailer-messages-api-openapi.yml
- filename: apollo-io-tasks-api-openapi.yml
  format: yaml
  label: Apollo.io Tasks API
  slug: apollo-io-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-tasks-api-openapi.yml
- filename: apollo-io-calls-api-openapi.yml
  format: yaml
  label: Apollo.io Calls API
  slug: apollo-io-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-calls-api-openapi.yml
- filename: apollo-io-conversations-api-openapi.yml
  format: yaml
  label: Apollo.io Conversations API
  slug: apollo-io-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-conversations-api-openapi.yml
- filename: apollo-io-analytics-api-openapi.yml
  format: yaml
  label: Apollo.io Analytics API
  slug: apollo-io-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-analytics-api-openapi.yml
- filename: apollo-io-fields-api-openapi.yml
  format: yaml
  label: Apollo.io Fields API
  slug: apollo-io-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-fields-api-openapi.yml
- filename: apollo-io-miscellaneous-api-openapi.yml
  format: yaml
  label: Apollo.io Miscellaneous API
  slug: apollo-io-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-miscellaneous-api-openapi.yml
- filename: apollo-io-users-api-openapi.yml
  format: yaml
  label: Apollo.io Users API
  slug: apollo-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apollo.io
  spf: true
hosts:
- cert_expires: Nov  9 12:24:25 2026 GMT
  host: www.apollo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 12:24:25 2026 GMT
  host: api.apollo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apollo Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apollo.io
provider_slug: apollo-io
slug: apollo-io-domain-security
source_filename: apollo-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 12:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 12:24:25 2026 GMT\n  hsts: null\ndomains:\n- domain: apollo.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/security/apollo-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Intelligence
- Prospecting
- Engagement
- B2B Data
- Enrichment
- CRM
- Sales Engagement
- Conversation Intelligence
- MCP
- Software-as-a-Service
---
