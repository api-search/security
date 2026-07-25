---
api_specs:
- filename: obol-address-api-openapi.yml
  format: yaml
  label: Obol Address API
  slug: obol-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-address-api-openapi.yml
- filename: obol-cluster-definition-api-openapi.yml
  format: yaml
  label: Obol Cluster Definition API
  slug: obol-cluster-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-cluster-definition-api-openapi.yml
- filename: obol-cluster-effectiveness-api-openapi.yml
  format: yaml
  label: Obol Cluster Effectiveness API
  slug: obol-cluster-effectiveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-cluster-effectiveness-api-openapi.yml
- filename: obol-cluster-lock-api-openapi.yml
  format: yaml
  label: Obol Cluster Lock API
  slug: obol-cluster-lock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-cluster-lock-api-openapi.yml
- filename: obol-deposit-data-api-openapi.yml
  format: yaml
  label: Obol Deposit Data API
  slug: obol-deposit-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-deposit-data-api-openapi.yml
- filename: obol-dv-exit-api-openapi.yml
  format: yaml
  label: Obol DV Exit API
  slug: obol-dv-exit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-dv-exit-api-openapi.yml
- filename: obol-dv-migrate-api-openapi.yml
  format: yaml
  label: Obol DV Migrate API
  slug: obol-dv-migrate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-dv-migrate-api-openapi.yml
- filename: obol-fee-recipient-api-openapi.yml
  format: yaml
  label: Obol Fee Recipient API
  slug: obol-fee-recipient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-fee-recipient-api-openapi.yml
- filename: obol-metrics-api-openapi.yml
  format: yaml
  label: Obol Metrics API
  slug: obol-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-metrics-api-openapi.yml
- filename: obol-owr-information-api-openapi.yml
  format: yaml
  label: Obol OWR Information API
  slug: obol-owr-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-owr-information-api-openapi.yml
- filename: obol-positions-api-openapi.yml
  format: yaml
  label: Obol Positions API
  slug: obol-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-positions-api-openapi.yml
- filename: obol-state-api-openapi.yml
  format: yaml
  label: Obol State API
  slug: obol-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-state-api-openapi.yml
- filename: obol-system-api-openapi.yml
  format: yaml
  label: Obol System API
  slug: obol-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-system-api-openapi.yml
- filename: obol-techne-credentials-api-openapi.yml
  format: yaml
  label: Obol Techne Credentials API
  slug: obol-techne-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-techne-credentials-api-openapi.yml
- filename: obol-terms-and-conditions-api-openapi.yml
  format: yaml
  label: Obol Terms And Conditions API
  slug: obol-terms-and-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-terms-and-conditions-api-openapi.yml
- filename: obol-test-api-openapi.yml
  format: yaml
  label: Obol Test API
  slug: obol-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-test-api-openapi.yml
- filename: obol-tvs-api-openapi.yml
  format: yaml
  label: Obol tvs API
  slug: obol-tvs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/openapi/obol-tvs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: obol.tech
  spf: true
hosts:
- cert_expires: Sep 29 00:14:31 2026 GMT
  host: obol.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Obol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Obol
provider_slug: obol
slug: obol-domain-security
source_filename: obol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obol.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:14:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: obol.tech\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obol/refs/heads/main/security/obol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Ethereum
- Staking
- Distributed Validators
- Blockchain Infrastructure
- Web3
---
