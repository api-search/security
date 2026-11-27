---
api_specs:
- filename: onboard-io-activity-api-openapi.yml
  format: yaml
  label: Onboard Activity API
  slug: onboard-io-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-activity-api-openapi.yml
- filename: onboard-io-assets-api-openapi.yml
  format: yaml
  label: Onboard Assets API
  slug: onboard-io-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-assets-api-openapi.yml
- filename: onboard-io-bots-api-openapi.yml
  format: yaml
  label: Onboard Bots API
  slug: onboard-io-bots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-bots-api-openapi.yml
- filename: onboard-io-comments-api-openapi.yml
  format: yaml
  label: Onboard Comments API
  slug: onboard-io-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-comments-api-openapi.yml
- filename: onboard-io-communication-records-api-openapi.yml
  format: yaml
  label: Onboard Communication Records API
  slug: onboard-io-communication-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-communication-records-api-openapi.yml
- filename: onboard-io-compliance-api-openapi.yml
  format: yaml
  label: Onboard Compliance API
  slug: onboard-io-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-compliance-api-openapi.yml
- filename: onboard-io-conversations-api-openapi.yml
  format: yaml
  label: Onboard Conversations API
  slug: onboard-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-conversations-api-openapi.yml
- filename: onboard-io-custom-api-openapi.yml
  format: yaml
  label: Onboard Custom API
  slug: onboard-io-custom-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-custom-api-openapi.yml
- filename: onboard-io-email-api-openapi.yml
  format: yaml
  label: Onboard Email API
  slug: onboard-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-email-api-openapi.yml
- filename: onboard-io-hooks-api-openapi.yml
  format: yaml
  label: Onboard Hooks API
  slug: onboard-io-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-hooks-api-openapi.yml
- filename: onboard-io-knowledge-base-api-openapi.yml
  format: yaml
  label: Onboard Knowledge Base API
  slug: onboard-io-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-knowledge-base-api-openapi.yml
- filename: onboard-io-map-api-openapi.yml
  format: yaml
  label: Onboard Map API
  slug: onboard-io-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-map-api-openapi.yml
- filename: onboard-io-platform-api-openapi.yml
  format: yaml
  label: Onboard Platform API
  slug: onboard-io-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-platform-api-openapi.yml
- filename: onboard-io-stats-api-openapi.yml
  format: yaml
  label: Onboard Stats API
  slug: onboard-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-stats-api-openapi.yml
- filename: onboard-io-workflows-api-openapi.yml
  format: yaml
  label: Onboard Workflows API
  slug: onboard-io-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: onboard.io
  spf: true
hosts:
- cert_expires: Jan 27 20:51:29 2027 GMT
  host: onboard.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Onboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Onboard
provider_slug: onboard-io
slug: onboard-io-domain-security
source_filename: onboard-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onboard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 20:51:29 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: onboard.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/onboard-io/security/onboard-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Customer Onboarding
- Software-as-a-Service
- B2B
- Integration
- Artificial Intelligence
---
