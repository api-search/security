---
api_specs:
- filename: shell-accounts-api-openapi.yml
  format: yaml
  label: Shell Accounts API
  slug: shell-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-accounts-api-openapi.yml
- filename: shell-cards-api-openapi.yml
  format: yaml
  label: Shell Cards API
  slug: shell-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-cards-api-openapi.yml
- filename: shell-catalogue-api-openapi.yml
  format: yaml
  label: Shell Catalogue API
  slug: shell-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-catalogue-api-openapi.yml
- filename: shell-invoices-api-openapi.yml
  format: yaml
  label: Shell Invoices API
  slug: shell-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-invoices-api-openapi.yml
- filename: shell-limits-api-openapi.yml
  format: yaml
  label: Shell Limits API
  slug: shell-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-limits-api-openapi.yml
- filename: shell-offers-api-openapi.yml
  format: yaml
  label: Shell Offers API
  slug: shell-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-offers-api-openapi.yml
- filename: shell-orders-api-openapi.yml
  format: yaml
  label: Shell Orders API
  slug: shell-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-orders-api-openapi.yml
- filename: shell-points-api-openapi.yml
  format: yaml
  label: Shell Points API
  slug: shell-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-points-api-openapi.yml
- filename: shell-products-api-openapi.yml
  format: yaml
  label: Shell Products API
  slug: shell-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-products-api-openapi.yml
- filename: shell-sites-api-openapi.yml
  format: yaml
  label: Shell Sites API
  slug: shell-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-sites-api-openapi.yml
- filename: shell-transactions-api-openapi.yml
  format: yaml
  label: Shell Transactions API
  slug: shell-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "entrust.net"
  - 0 issue "symantec.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "www.digicert.com"
  - 0 issuemail "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: shell.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.shell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: developer.shell.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.shell.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Shell
provider_slug: shell
slug: shell-domain-security
source_filename: shell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.shell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.shell.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shell.com\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"symantec.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issuemail \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/security/shell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Aviation
- Electric Vehicle Charging
- Energy
- Fleet Management
- Fuel
- Gas
- Loyalty
- Lubricants
- Mobility
- Oil and Gas
- Renewable Energy
---
