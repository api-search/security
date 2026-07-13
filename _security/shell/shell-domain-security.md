---
api_specs:
- filename: shell-b2b-mobility-openapi.yml
  format: yaml
  label: Shell B2B Mobility Card Management API
  slug: b2b-mobility-card-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-b2b-mobility-openapi.yml
- filename: shell-b2b-mobility-openapi.yml
  format: yaml
  label: Shell B2B Mobility Card Transaction Data API
  slug: b2b-mobility-card-transaction-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-b2b-mobility-openapi.yml
- filename: shell-b2b-mobility-openapi.yml
  format: yaml
  label: Shell B2B Mobility Invoice API
  slug: b2b-mobility-invoice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-b2b-mobility-openapi.yml
- filename: shell-loyalty-openapi.yml
  format: yaml
  label: Shell Loyalty Catalogue API
  slug: loyalty-catalogue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-loyalty-openapi.yml
- filename: shell-loyalty-openapi.yml
  format: yaml
  label: Shell Loyalty Account Management API
  slug: loyalty-account-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-loyalty-openapi.yml
- filename: shell-loyalty-openapi.yml
  format: yaml
  label: Shell Loyalty Points Balance API
  slug: loyalty-points-balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-loyalty-openapi.yml
- filename: shell-loyalty-openapi.yml
  format: yaml
  label: Shell Loyalty Points Redemption API
  slug: loyalty-points-redemption
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-loyalty-openapi.yml
- filename: shell-lubricants-openapi.yml
  format: yaml
  label: Shell Lubricants Order Management API
  slug: lubricants-order-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-lubricants-openapi.yml
- filename: shell-b2b-mobility-openapi.yml
  format: yaml
  label: Shell B2B Mobility Sites API
  slug: b2b-mobility-sites
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shell/refs/heads/main/openapi/shell-b2b-mobility-openapi.yml
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
