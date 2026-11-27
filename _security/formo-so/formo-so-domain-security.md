---
api_specs:
- filename: formo-so-alerts-api-openapi.yml
  format: yaml
  label: Formo Alerts API
  slug: formo-so-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-alerts-api-openapi.yml
- filename: formo-so-boards-api-openapi.yml
  format: yaml
  label: Formo Boards API
  slug: formo-so-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-boards-api-openapi.yml
- filename: formo-so-charts-api-openapi.yml
  format: yaml
  label: Formo Charts API
  slug: formo-so-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-charts-api-openapi.yml
- filename: formo-so-contracts-api-openapi.yml
  format: yaml
  label: Formo Contracts API
  slug: formo-so-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-contracts-api-openapi.yml
- filename: formo-so-events-api-openapi.yml
  format: yaml
  label: Formo Events API
  slug: formo-so-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-events-api-openapi.yml
- filename: formo-so-profiles-api-openapi.yml
  format: yaml
  label: Formo Profiles API
  slug: formo-so-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-profiles-api-openapi.yml
- filename: formo-so-query-api-openapi.yml
  format: yaml
  label: Formo Query API
  slug: formo-so-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-query-api-openapi.yml
- filename: formo-so-segments-api-openapi.yml
  format: yaml
  label: Formo Segments API
  slug: formo-so-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formo-so/openapi/formo-so-segments-api-openapi.yml
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
  domain: formo.so
  spf: true
hosts:
- cert_expires: Jan 14 18:06:25 2027 GMT
  host: formo.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Formo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Formo
provider_slug: formo-so
slug: formo-so-domain-security
source_filename: formo-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formo.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 18:06:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: formo.so\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/formo-so/security/formo-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Attribution
- Cryptocurrency
- DeFi
- Wallet Intelligence
- Token‑Gated Forms
- AI Agents
---
