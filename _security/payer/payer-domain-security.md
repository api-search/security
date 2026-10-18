---
api_specs:
- filename: payer-all-api-openapi.yml
  format: yaml
  label: Payer All API
  slug: payer-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-all-api-openapi.yml
- filename: payer-audit-api-openapi.yml
  format: yaml
  label: Payer Audit API
  slug: payer-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-audit-api-openapi.yml
- filename: payer-changelog-api-openapi.yml
  format: yaml
  label: Payer Changelog API
  slug: payer-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-changelog-api-openapi.yml
- filename: payer-documentation-api-openapi.yml
  format: yaml
  label: Payer Documentation API
  slug: payer-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-documentation-api-openapi.yml
- filename: payer-events-api-openapi.yml
  format: yaml
  label: Payer Events API
  slug: payer-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-events-api-openapi.yml
- filename: payer-export-api-openapi.yml
  format: yaml
  label: Payer Export API
  slug: payer-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-export-api-openapi.yml
- filename: payer-invoices-api-openapi.yml
  format: yaml
  label: Payer Invoices API
  slug: payer-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-invoices-api-openapi.yml
- filename: payer-oauth2-api-openapi.yml
  format: yaml
  label: Payer Oauth2 API
  slug: payer-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-oauth2-api-openapi.yml
- filename: payer-orders-api-openapi.yml
  format: yaml
  label: Payer Orders API
  slug: payer-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-orders-api-openapi.yml
- filename: payer-page-api-openapi.yml
  format: yaml
  label: Payer Page API
  slug: payer-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-page-api-openapi.yml
- filename: payer-payer-api-api-openapi.yml
  format: yaml
  label: Payer Payer API
  slug: payer-payer-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-payer-api-api-openapi.yml
- filename: payer-reader-access-api-openapi.yml
  format: yaml
  label: Payer Reader Access API
  slug: payer-reader-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-reader-access-api-openapi.yml
- filename: payer-reference-api-openapi.yml
  format: yaml
  label: Payer Reference API
  slug: payer-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-reference-api-openapi.yml
- filename: payer-search-api-openapi.yml
  format: yaml
  label: Payer Search API
  slug: payer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-search-api-openapi.yml
- filename: payer-users-api-openapi.yml
  format: yaml
  label: Payer Users API
  slug: payer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-users-api-openapi.yml
- filename: payer-version-api-openapi.yml
  format: yaml
  label: Payer Version API
  slug: payer-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: payer.eu
  spf: false
hosts:
- cert_expires: Nov 26 22:06:43 2026 GMT
  host: payer.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Payer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Payer
provider_slug: payer
slug: payer-domain-security
source_filename: payer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payer.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 22:06:43 2026 GMT\n  hsts: false\ndomains:\n- domain: payer.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/security/payer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- B2B
- Fintech
- Automation
---
