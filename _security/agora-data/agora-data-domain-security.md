---
api_specs:
- filename: agora-data-health-api-openapi.yml
  format: yaml
  label: Agora Data Health API
  slug: agora-data-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-health-api-openapi.yml
- filename: agora-data-hooks-api-openapi.yml
  format: yaml
  label: Agora Data Hooks API
  slug: agora-data-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-hooks-api-openapi.yml
- filename: agora-data-import-api-openapi.yml
  format: yaml
  label: Agora Data Import API
  slug: agora-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-import-api-openapi.yml
- filename: agora-data-inventory-api-openapi.yml
  format: yaml
  label: Agora Data Inventory API
  slug: agora-data-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-inventory-api-openapi.yml
- filename: agora-data-loans-api-openapi.yml
  format: yaml
  label: Agora Data Loans API
  slug: agora-data-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-loans-api-openapi.yml
- filename: agora-data-login-api-openapi.yml
  format: yaml
  label: Agora Data Login API
  slug: agora-data-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-login-api-openapi.yml
- filename: agora-data-oauth-api-openapi.yml
  format: yaml
  label: Agora Data OAUTH API
  slug: agora-data-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-oauth-api-openapi.yml
- filename: agora-data-providers-api-openapi.yml
  format: yaml
  label: Agora Data Providers API
  slug: agora-data-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-providers-api-openapi.yml
- filename: agora-data-status-api-openapi.yml
  format: yaml
  label: Agora Data Status API
  slug: agora-data-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-status-api-openapi.yml
- filename: agora-data-uploads-api-openapi.yml
  format: yaml
  label: Agora Data Uploads API
  slug: agora-data-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-uploads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agoradata.com
  spf: true
hosts:
- cert_expires: Oct  1 11:29:31 2026 GMT
  host: agoradata.com
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.agoradata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agora Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agora Data, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agora Data
provider_slug: agora-data
slug: agora-data-domain-security
source_filename: agora-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agoradata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:29:31 2026 GMT\n  hsts: true\n- host: api.agoradata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: agoradata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/security/agora-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Auto Finance
- Automotive
- Lending
- Financial-Services
- Fintech
- Loan Origination
- Data Analytics
- Artificial Intelligence
- Capital Markets
---
