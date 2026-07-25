---
api_specs:
- filename: elliptic-assets-api-openapi.yml
  format: yaml
  label: Elliptic Assets API
  slug: elliptic-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-assets-api-openapi.yml
- filename: elliptic-count-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Count Analyses API
  slug: elliptic-count-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-count-analyses-api-openapi.yml
- filename: elliptic-criteria-api-openapi.yml
  format: yaml
  label: Elliptic Criteria API
  slug: elliptic-criteria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-criteria-api-openapi.yml
- filename: elliptic-customers-api-openapi.yml
  format: yaml
  label: Elliptic Customers API
  slug: elliptic-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-customers-api-openapi.yml
- filename: elliptic-health-api-openapi.yml
  format: yaml
  label: Elliptic Health API
  slug: elliptic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-health-api-openapi.yml
- filename: elliptic-risk-rules-api-openapi.yml
  format: yaml
  label: Elliptic Risk Rules API
  slug: elliptic-risk-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-risk-rules-api-openapi.yml
- filename: elliptic-sanctions-api-openapi.yml
  format: yaml
  label: Elliptic Sanctions API
  slug: elliptic-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-sanctions-api-openapi.yml
- filename: elliptic-screenings-api-openapi.yml
  format: yaml
  label: Elliptic Screenings API
  slug: elliptic-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-screenings-api-openapi.yml
- filename: elliptic-transaction-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Transaction Analyses API
  slug: elliptic-transaction-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-transaction-analyses-api-openapi.yml
- filename: elliptic-transaction-workflow-api-openapi.yml
  format: yaml
  label: Elliptic Transaction Workflow API
  slug: elliptic-transaction-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-transaction-workflow-api-openapi.yml
- filename: elliptic-tron-nodeintelligence-api-openapi.yml
  format: yaml
  label: Elliptic Tron NodeIntelligence API
  slug: elliptic-tron-nodeintelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-tron-nodeintelligence-api-openapi.yml
- filename: elliptic-users-api-openapi.yml
  format: yaml
  label: Elliptic Users API
  slug: elliptic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-users-api-openapi.yml
- filename: elliptic-wallet-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Analyses API
  slug: elliptic-wallet-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-analyses-api-openapi.yml
- filename: elliptic-wallet-analyses-count-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Analyses Count API
  slug: elliptic-wallet-analyses-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-analyses-count-api-openapi.yml
- filename: elliptic-wallet-api-openapi.yml
  format: yaml
  label: Elliptic Wallet API
  slug: elliptic-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-api-openapi.yml
- filename: elliptic-wallet-workflow-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Workflow API
  slug: elliptic-wallet-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-workflow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elliptic.co
  spf: true
hosts:
- cert_expires: Sep 11 18:42:23 2026 GMT
  host: developers.elliptic.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: aml-api.elliptic.co
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: sanctions-api.elliptic.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elliptic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elliptic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elliptic
provider_slug: elliptic
slug: elliptic-domain-security
source_filename: elliptic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.elliptic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:42:23 2026 GMT\n  hsts: null\n- host: aml-api.elliptic.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\n- host: sanctions-api.elliptic.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: elliptic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/security/elliptic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Blockchain
- Crypto
- Compliance
- AML
- Transaction Screening
- Wallet Screening
- Risk Scoring
- Analytics
---
