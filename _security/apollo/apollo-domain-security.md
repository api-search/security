---
api_specs:
- filename: apollo-accounts-api-openapi.yml
  format: yaml
  label: Apollo Accounts API
  slug: apollo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-accounts-api-openapi.yml
- filename: apollo-contacts-api-openapi.yml
  format: yaml
  label: Apollo Contacts API
  slug: apollo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-contacts-api-openapi.yml
- filename: apollo-email-accounts-api-openapi.yml
  format: yaml
  label: Apollo Email Accounts API
  slug: apollo-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-email-accounts-api-openapi.yml
- filename: apollo-emailer-campaigns-api-openapi.yml
  format: yaml
  label: Apollo Emailer Campaigns API
  slug: apollo-emailer-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-emailer-campaigns-api-openapi.yml
- filename: apollo-mixed-companies-api-openapi.yml
  format: yaml
  label: Apollo Mixed Companies API
  slug: apollo-mixed-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-mixed-companies-api-openapi.yml
- filename: apollo-mixed-people-api-openapi.yml
  format: yaml
  label: Apollo Mixed People API
  slug: apollo-mixed-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-mixed-people-api-openapi.yml
- filename: apollo-opportunities-api-openapi.yml
  format: yaml
  label: Apollo Opportunities API
  slug: apollo-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-opportunities-api-openapi.yml
- filename: apollo-organizations-api-openapi.yml
  format: yaml
  label: Apollo Organizations API
  slug: apollo-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-organizations-api-openapi.yml
- filename: apollo-people-api-openapi.yml
  format: yaml
  label: Apollo People API
  slug: apollo-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-people-api-openapi.yml
- filename: apollo-phone-calls-api-openapi.yml
  format: yaml
  label: Apollo Phone Calls API
  slug: apollo-phone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-phone-calls-api-openapi.yml
- filename: apollo-sync-report-api-openapi.yml
  format: yaml
  label: Apollo Sync Report API
  slug: apollo-sync-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-sync-report-api-openapi.yml
- filename: apollo-tasks-api-openapi.yml
  format: yaml
  label: Apollo Tasks API
  slug: apollo-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-tasks-api-openapi.yml
- filename: apollo-usage-stats-api-openapi.yml
  format: yaml
  label: Apollo Usage Stats API
  slug: apollo-usage-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-usage-stats-api-openapi.yml
- filename: apollo-users-api-openapi.yml
  format: yaml
  label: Apollo Users API
  slug: apollo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/openapi/apollo-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apollo.io
  spf: true
hosts:
- cert_expires: Sep 11 12:03:29 2026 GMT
  host: www.apollo.io
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
name: Apollo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apollo
provider_slug: apollo
slug: apollo-domain-security
source_filename: apollo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:03:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:03:29 2026 GMT\n  hsts: null\ndomains:\n- domain: apollo.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo/refs/heads/main/security/apollo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- B2B Sales
- CRM
- Data Enrichment
- Lead Generation
- Sales Intelligence
- Sales Platform
---
