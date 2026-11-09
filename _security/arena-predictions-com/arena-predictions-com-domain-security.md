---
api_specs:
- filename: arena-predictions-com-api-keys-api-openapi.yml
  format: yaml
  label: Arena API keys API
  slug: arena-predictions-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-api-keys-api-openapi.yml
- filename: arena-predictions-com-identity-api-openapi.yml
  format: yaml
  label: Arena Identity API
  slug: arena-predictions-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-identity-api-openapi.yml
- filename: arena-predictions-com-markets-api-openapi.yml
  format: yaml
  label: Arena Markets API
  slug: arena-predictions-com-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-markets-api-openapi.yml
- filename: arena-predictions-com-portfolio-api-openapi.yml
  format: yaml
  label: Arena Portfolio API
  slug: arena-predictions-com-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-portfolio-api-openapi.yml
- filename: arena-predictions-com-records-api-openapi.yml
  format: yaml
  label: Arena Records API
  slug: arena-predictions-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-records-api-openapi.yml
- filename: arena-predictions-com-status-api-openapi.yml
  format: yaml
  label: Arena Status API
  slug: arena-predictions-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-status-api-openapi.yml
- filename: arena-predictions-com-trading-api-openapi.yml
  format: yaml
  label: Arena Trading API
  slug: arena-predictions-com-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-trading-api-openapi.yml
- filename: arena-predictions-com-usage-api-openapi.yml
  format: yaml
  label: Arena Usage API
  slug: arena-predictions-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-usage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: arena-predictions.com
  spf: false
hosts:
- cert_expires: Dec 19 11:40:28 2026 GMT
  host: arena-predictions.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arena Predictions Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arena, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Arena
provider_slug: arena-predictions-com
slug: arena-predictions-com-domain-security
source_filename: arena-predictions-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arena-predictions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 11:40:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arena-predictions.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/arena-predictions-com/security/arena-predictions-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Prediction Markets
- Paper Trading
- Sandbox
- CLI
---
