---
api_specs:
- filename: anteproof-com-account-api-openapi.yml
  format: yaml
  label: Anteproof Account API
  slug: anteproof-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-account-api-openapi.yml
- filename: anteproof-com-anchor-api-openapi.yml
  format: yaml
  label: Anteproof Anchor API
  slug: anteproof-com-anchor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-anchor-api-openapi.yml
- filename: anteproof-com-billing-api-openapi.yml
  format: yaml
  label: Anteproof Billing API
  slug: anteproof-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-billing-api-openapi.yml
- filename: anteproof-com-calibration-api-openapi.yml
  format: yaml
  label: Anteproof Calibration API
  slug: anteproof-com-calibration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-calibration-api-openapi.yml
- filename: anteproof-com-chain-api-openapi.yml
  format: yaml
  label: Anteproof Chain API
  slug: anteproof-com-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-chain-api-openapi.yml
- filename: anteproof-com-coverage-preview-api-openapi.yml
  format: yaml
  label: Anteproof Coverage Preview API
  slug: anteproof-com-coverage-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-coverage-preview-api-openapi.yml
- filename: anteproof-com-digest-api-openapi.yml
  format: yaml
  label: Anteproof Digest API
  slug: anteproof-com-digest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-digest-api-openapi.yml
- filename: anteproof-com-entities-api-openapi.yml
  format: yaml
  label: Anteproof Entities API
  slug: anteproof-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-entities-api-openapi.yml
- filename: anteproof-com-forecasts-api-openapi.yml
  format: yaml
  label: Anteproof Forecasts API
  slug: anteproof-com-forecasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-forecasts-api-openapi.yml
- filename: anteproof-com-freshness-api-openapi.yml
  format: yaml
  label: Anteproof Freshness API
  slug: anteproof-com-freshness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-freshness-api-openapi.yml
- filename: anteproof-com-me-api-openapi.yml
  format: yaml
  label: Anteproof Me API
  slug: anteproof-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-me-api-openapi.yml
- filename: anteproof-com-proof-api-openapi.yml
  format: yaml
  label: Anteproof Proof API
  slug: anteproof-com-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-proof-api-openapi.yml
- filename: anteproof-com-questions-api-openapi.yml
  format: yaml
  label: Anteproof Questions API
  slug: anteproof-com-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-questions-api-openapi.yml
- filename: anteproof-com-risk-api-openapi.yml
  format: yaml
  label: Anteproof Risk API
  slug: anteproof-com-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-risk-api-openapi.yml
- filename: anteproof-com-stats-api-openapi.yml
  format: yaml
  label: Anteproof Stats API
  slug: anteproof-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-stats-api-openapi.yml
- filename: anteproof-com-support-api-openapi.yml
  format: yaml
  label: Anteproof Support API
  slug: anteproof-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anteproof-com/openapi/anteproof-com-support-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anteproof.com
  spf: true
hosts:
- cert_expires: Jan 29 15:49:59 2027 GMT
  host: anteproof.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anteproof Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anteproof, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anteproof
provider_slug: anteproof-com
slug: anteproof-com-domain-security
source_filename: anteproof-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anteproof.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 15:49:59 2027 GMT\n  hsts: null\ndomains:\n- domain: anteproof.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anteproof-com/security/anteproof-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Dependency
- Risk Management
- Analytics
- Open Source
- Software
---
