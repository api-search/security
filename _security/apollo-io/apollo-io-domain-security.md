---
api_specs:
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
- filename: apollo-io-email-accounts-api-openapi.yml
  format: yaml
  label: Apollo.io Email Accounts API
  slug: apollo-io-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-email-accounts-api-openapi.yml
- filename: apollo-io-emailer-campaigns-api-openapi.yml
  format: yaml
  label: Apollo.io Emailer Campaigns API
  slug: apollo-io-emailer-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-emailer-campaigns-api-openapi.yml
- filename: apollo-io-mixed-companies-api-openapi.yml
  format: yaml
  label: Apollo.io Mixed Companies API
  slug: apollo-io-mixed-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-mixed-companies-api-openapi.yml
- filename: apollo-io-mixed-people-api-openapi.yml
  format: yaml
  label: Apollo.io Mixed People API
  slug: apollo-io-mixed-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-mixed-people-api-openapi.yml
- filename: apollo-io-opportunities-api-openapi.yml
  format: yaml
  label: Apollo.io Opportunities API
  slug: apollo-io-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-opportunities-api-openapi.yml
- filename: apollo-io-organizations-api-openapi.yml
  format: yaml
  label: Apollo.io Organizations API
  slug: apollo-io-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-organizations-api-openapi.yml
- filename: apollo-io-people-api-openapi.yml
  format: yaml
  label: Apollo.io People API
  slug: apollo-io-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-people-api-openapi.yml
- filename: apollo-io-phone-calls-api-openapi.yml
  format: yaml
  label: Apollo.io Phone Calls API
  slug: apollo-io-phone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-phone-calls-api-openapi.yml
- filename: apollo-io-sync-report-api-openapi.yml
  format: yaml
  label: Apollo.io Sync Report API
  slug: apollo-io-sync-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-sync-report-api-openapi.yml
- filename: apollo-io-tasks-api-openapi.yml
  format: yaml
  label: Apollo.io Tasks API
  slug: apollo-io-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-tasks-api-openapi.yml
- filename: apollo-io-usage-stats-api-openapi.yml
  format: yaml
  label: Apollo.io Usage Stats API
  slug: apollo-io-usage-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-usage-stats-api-openapi.yml
- filename: apollo-io-users-api-openapi.yml
  format: yaml
  label: Apollo.io Users API
  slug: apollo-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-users-api-openapi.yml
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
name: Apollo Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apollo.io
provider_slug: apollo-io
slug: apollo-io-domain-security
source_filename: apollo-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:03:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apollo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:03:29 2026 GMT\n  hsts: null\ndomains:\n- domain: apollo.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/security/apollo-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Intelligence
- Prospecting
- Engagement
- B2B Data
- Enrichment
- SaaS
---
