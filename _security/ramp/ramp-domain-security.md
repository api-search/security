---
api_specs:
- filename: ramp-accounts-api-openapi.yml
  format: yaml
  label: Ramp Accounts API
  slug: ramp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-accounts-api-openapi.yml
- filename: ramp-audit-logs-api-openapi.yml
  format: yaml
  label: Ramp Audit Logs API
  slug: ramp-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-audit-logs-api-openapi.yml
- filename: ramp-bills-api-openapi.yml
  format: yaml
  label: Ramp Bills API
  slug: ramp-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-bills-api-openapi.yml
- filename: ramp-cards-api-openapi.yml
  format: yaml
  label: Ramp Cards API
  slug: ramp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-cards-api-openapi.yml
- filename: ramp-departments-api-openapi.yml
  format: yaml
  label: Ramp Departments API
  slug: ramp-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-departments-api-openapi.yml
- filename: ramp-locations-api-openapi.yml
  format: yaml
  label: Ramp Locations API
  slug: ramp-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-locations-api-openapi.yml
- filename: ramp-reimbursements-api-openapi.yml
  format: yaml
  label: Ramp Reimbursements API
  slug: ramp-reimbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-reimbursements-api-openapi.yml
- filename: ramp-statements-api-openapi.yml
  format: yaml
  label: Ramp Statements API
  slug: ramp-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-statements-api-openapi.yml
- filename: ramp-transactions-api-openapi.yml
  format: yaml
  label: Ramp Transactions API
  slug: ramp-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-transactions-api-openapi.yml
- filename: ramp-users-api-openapi.yml
  format: yaml
  label: Ramp Users API
  slug: ramp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-users-api-openapi.yml
- filename: ramp-vendors-api-openapi.yml
  format: yaml
  label: Ramp Vendors API
  slug: ramp-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-vendors-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ramp.com
  spf: true
hosts:
- cert_expires: Oct  6 03:30:50 2026 GMT
  host: ramp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:20:50 2026 GMT
  host: docs.ramp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 03:30:50 2026 GMT
  host: api.ramp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ramp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ramp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ramp
provider_slug: ramp
slug: ramp-domain-security
source_filename: ramp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:20:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:30:50 2026 GMT\n  hsts: null\ndomains:\n- domain: ramp.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/security/ramp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Spend Management
- Corporate Cards
- Expense Management
- Accounts Payable
- Bill Pay
- Accounting
- Reimbursements
---
