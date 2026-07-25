---
api_specs:
- filename: fyle-advances-api-openapi.yml
  format: yaml
  label: Fyle Advances API
  slug: fyle-advances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-advances-api-openapi.yml
- filename: fyle-categories-api-openapi.yml
  format: yaml
  label: Fyle Categories API
  slug: fyle-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-categories-api-openapi.yml
- filename: fyle-corporate-cards-api-openapi.yml
  format: yaml
  label: Fyle Corporate Cards API
  slug: fyle-corporate-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-corporate-cards-api-openapi.yml
- filename: fyle-cost-centers-api-openapi.yml
  format: yaml
  label: Fyle Cost Centers API
  slug: fyle-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-cost-centers-api-openapi.yml
- filename: fyle-employees-api-openapi.yml
  format: yaml
  label: Fyle Employees API
  slug: fyle-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-employees-api-openapi.yml
- filename: fyle-expenses-api-openapi.yml
  format: yaml
  label: Fyle Expenses API
  slug: fyle-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-expenses-api-openapi.yml
- filename: fyle-files-api-openapi.yml
  format: yaml
  label: Fyle Files API
  slug: fyle-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-files-api-openapi.yml
- filename: fyle-merchants-api-openapi.yml
  format: yaml
  label: Fyle Merchants API
  slug: fyle-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-merchants-api-openapi.yml
- filename: fyle-projects-api-openapi.yml
  format: yaml
  label: Fyle Projects API
  slug: fyle-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-projects-api-openapi.yml
- filename: fyle-reports-api-openapi.yml
  format: yaml
  label: Fyle Reports API
  slug: fyle-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-reports-api-openapi.yml
- filename: fyle-webhooks-api-openapi.yml
  format: yaml
  label: Fyle Webhooks API
  slug: fyle-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/openapi/fyle-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fylehq.com
  spf: true
hosts:
- cert_expires: Aug 22 05:01:03 2026 GMT
  host: www.fylehq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:33:01 2026 GMT
  host: docs.fylehq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.fylehq.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fyle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fyle, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fyle
provider_slug: fyle
slug: fyle-domain-security
source_filename: fyle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fylehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:01:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fylehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:33:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fylehq.com\n  https: false\ndomains:\n- domain: fylehq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fyle/refs/heads/main/security/fyle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Expense Management
- Spend Management
- Corporate Cards
- Fintech
- Accounting
- Receipts
---
