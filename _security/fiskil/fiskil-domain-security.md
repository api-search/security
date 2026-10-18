---
api_specs:
- filename: fiskil-auth-api-openapi.yml
  format: yaml
  label: FISKIL Auth API
  slug: fiskil-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-auth-api-openapi.yml
- filename: fiskil-banking-api-openapi.yml
  format: yaml
  label: FISKIL Banking API
  slug: fiskil-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-banking-api-openapi.yml
- filename: fiskil-common-api-openapi.yml
  format: yaml
  label: FISKIL Common API
  slug: fiskil-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-common-api-openapi.yml
- filename: fiskil-consent-api-openapi.yml
  format: yaml
  label: FISKIL Consent API
  slug: fiskil-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-consent-api-openapi.yml
- filename: fiskil-end-users-api-openapi.yml
  format: yaml
  label: FISKIL End users API
  slug: fiskil-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-end-users-api-openapi.yml
- filename: fiskil-energy-api-openapi.yml
  format: yaml
  label: FISKIL Energy API
  slug: fiskil-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-energy-api-openapi.yml
- filename: fiskil-institutions-api-openapi.yml
  format: yaml
  label: FISKIL Institutions API
  slug: fiskil-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-institutions-api-openapi.yml
- filename: fiskil-transactions-api-openapi.yml
  format: yaml
  label: FISKIL Transactions API
  slug: fiskil-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fiskil.com
  spf: true
hosts:
- cert_expires: Dec  7 02:56:15 2026 GMT
  host: www.fiskil.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fiskil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FISKIL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FISKIL
provider_slug: fiskil
slug: fiskil-domain-security
source_filename: fiskil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fiskil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 02:56:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fiskil.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/security/fiskil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Banking
- Data Sharing
- Financial Services
- API Platform
- North America
---
