---
api_specs:
- filename: splitwise-comments-api-openapi.yml
  format: yaml
  label: Splitwise comments API
  slug: splitwise-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-comments-api-openapi.yml
- filename: splitwise-expenses-api-openapi.yml
  format: yaml
  label: Splitwise expenses API
  slug: splitwise-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-expenses-api-openapi.yml
- filename: splitwise-friends-api-openapi.yml
  format: yaml
  label: Splitwise friends API
  slug: splitwise-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-friends-api-openapi.yml
- filename: splitwise-groups-api-openapi.yml
  format: yaml
  label: Splitwise groups API
  slug: splitwise-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-groups-api-openapi.yml
- filename: splitwise-notifications-api-openapi.yml
  format: yaml
  label: Splitwise notifications API
  slug: splitwise-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-notifications-api-openapi.yml
- filename: splitwise-other-api-openapi.yml
  format: yaml
  label: Splitwise other API
  slug: splitwise-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-other-api-openapi.yml
- filename: splitwise-users-api-openapi.yml
  format: yaml
  label: Splitwise users API
  slug: splitwise-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:ops@splitwise.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: splitwise.com
  spf: true
hosts:
- cert_expires: Sep 26 13:22:53 2026 GMT
  host: www.splitwise.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Splitwise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splitwise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Splitwise
provider_slug: splitwise
slug: splitwise-domain-security
source_filename: splitwise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.splitwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: splitwise.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:ops@splitwise.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/security/splitwise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Expense Management
- Personal Finance
- Bill Splitting
- Payments
- REST API
- OAuth
---
