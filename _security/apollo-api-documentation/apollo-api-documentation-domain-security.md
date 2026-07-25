---
api_specs:
- filename: apollo-api-documentation-accounts-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Accounts API
  slug: apollo-api-documentation-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-accounts-api-openapi.yml
- filename: apollo-api-documentation-contacts-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Contacts API
  slug: apollo-api-documentation-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-contacts-api-openapi.yml
- filename: apollo-api-documentation-email-accounts-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Email Accounts API
  slug: apollo-api-documentation-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-email-accounts-api-openapi.yml
- filename: apollo-api-documentation-emailer-campaigns-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Emailer Campaigns API
  slug: apollo-api-documentation-emailer-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-emailer-campaigns-api-openapi.yml
- filename: apollo-api-documentation-mixed-companies-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Mixed Companies API
  slug: apollo-api-documentation-mixed-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-mixed-companies-api-openapi.yml
- filename: apollo-api-documentation-mixed-people-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Mixed People API
  slug: apollo-api-documentation-mixed-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-mixed-people-api-openapi.yml
- filename: apollo-api-documentation-opportunities-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Opportunities API
  slug: apollo-api-documentation-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-opportunities-api-openapi.yml
- filename: apollo-api-documentation-organizations-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Organizations API
  slug: apollo-api-documentation-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-organizations-api-openapi.yml
- filename: apollo-api-documentation-people-api-openapi.yml
  format: yaml
  label: Apollo API Documentation People API
  slug: apollo-api-documentation-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-people-api-openapi.yml
- filename: apollo-api-documentation-phone-calls-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Phone Calls API
  slug: apollo-api-documentation-phone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-phone-calls-api-openapi.yml
- filename: apollo-api-documentation-sync-report-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Sync Report API
  slug: apollo-api-documentation-sync-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-sync-report-api-openapi.yml
- filename: apollo-api-documentation-tasks-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Tasks API
  slug: apollo-api-documentation-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-tasks-api-openapi.yml
- filename: apollo-api-documentation-usage-stats-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Usage Stats API
  slug: apollo-api-documentation-usage-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-usage-stats-api-openapi.yml
- filename: apollo-api-documentation-users-api-openapi.yml
  format: yaml
  label: Apollo API Documentation Users API
  slug: apollo-api-documentation-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
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
- cert_expires: Sep 11 12:03:29 2026 GMT
  host: api.apollo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apollo Api Documentation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo API Documentation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apollo API Documentation
provider_slug: apollo-api-documentation
slug: apollo-api-documentation-domain-security
source_filename: apollo-api-documentation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:03:29 2026 GMT\n  hsts: null\ndomains:\n- domain: apollo.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/security/apollo-api-documentation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Documentation
- Best Practices
- Data Enrichment
- People Search
- Sales Intelligence
---
