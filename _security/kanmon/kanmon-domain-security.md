---
api_specs:
- filename: kanmon-bank-accounts-api-openapi.yml
  format: yaml
  label: Kanmon Bank Accounts API
  slug: kanmon-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-bank-accounts-api-openapi.yml
- filename: kanmon-businesses-api-openapi.yml
  format: yaml
  label: Kanmon Businesses API
  slug: kanmon-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-businesses-api-openapi.yml
- filename: kanmon-connect-tokens-api-openapi.yml
  format: yaml
  label: Kanmon Connect Tokens API
  slug: kanmon-connect-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-connect-tokens-api-openapi.yml
- filename: kanmon-documents-api-openapi.yml
  format: yaml
  label: Kanmon Documents API
  slug: kanmon-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-documents-api-openapi.yml
- filename: kanmon-draw-requests-api-openapi.yml
  format: yaml
  label: Kanmon Draw Requests API
  slug: kanmon-draw-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-draw-requests-api-openapi.yml
- filename: kanmon-embedded-sessions-api-openapi.yml
  format: yaml
  label: Kanmon Embedded Sessions API
  slug: kanmon-embedded-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-embedded-sessions-api-openapi.yml
- filename: kanmon-integrated-mca-api-openapi.yml
  format: yaml
  label: Kanmon Integrated MCA API
  slug: kanmon-integrated-mca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-integrated-mca-api-openapi.yml
- filename: kanmon-invoices-api-openapi.yml
  format: yaml
  label: Kanmon Invoices API
  slug: kanmon-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-invoices-api-openapi.yml
- filename: kanmon-issued-products-api-openapi.yml
  format: yaml
  label: Kanmon Issued Products API
  slug: kanmon-issued-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-issued-products-api-openapi.yml
- filename: kanmon-offers-api-openapi.yml
  format: yaml
  label: Kanmon Offers API
  slug: kanmon-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-offers-api-openapi.yml
- filename: kanmon-payments-api-openapi.yml
  format: yaml
  label: Kanmon Payments API
  slug: kanmon-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-payments-api-openapi.yml
- filename: kanmon-prequalifications-api-openapi.yml
  format: yaml
  label: Kanmon Prequalifications API
  slug: kanmon-prequalifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-prequalifications-api-openapi.yml
- filename: kanmon-sandbox-utilities-api-openapi.yml
  format: yaml
  label: Kanmon Sandbox Utilities API
  slug: kanmon-sandbox-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-sandbox-utilities-api-openapi.yml
- filename: kanmon-users-api-openapi.yml
  format: yaml
  label: Kanmon Users API
  slug: kanmon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kanmonhq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kanmon.com
  spf: true
hosts:
- cert_expires: Sep  1 05:23:27 2026 GMT
  host: www.kanmonhq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 22:43:09 2026 GMT
  host: api.kanmon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 18:23:29 2026 GMT
  host: api.kanmon.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kanmon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kanmon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kanmon
provider_slug: kanmon
slug: kanmon-domain-security
source_filename: kanmon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kanmonhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 05:23:27 2026 GMT\n  hsts: null\n- host: api.kanmon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:43:09 2026 GMT\n  hsts: null\n- host: api.kanmon.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 18:23:29 2026 GMT\n  hsts: null\ndomains:\n- domain: kanmonhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kanmon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/security/kanmon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Embedded Finance
- Embedded Lending
- Lending
- Working Capital
- Invoice Financing
---
