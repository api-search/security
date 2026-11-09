---
api_specs:
- filename: capgo-app-api-keys-api-openapi.yml
  format: yaml
  label: Capgo API Keys API
  slug: capgo-app-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-api-keys-api-openapi.yml
- filename: capgo-app-apps-api-openapi.yml
  format: yaml
  label: Capgo Apps API
  slug: capgo-app-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-apps-api-openapi.yml
- filename: capgo-app-bundles-api-openapi.yml
  format: yaml
  label: Capgo Bundles API
  slug: capgo-app-bundles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-bundles-api-openapi.yml
- filename: capgo-app-channels-api-openapi.yml
  format: yaml
  label: Capgo Channels API
  slug: capgo-app-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-channels-api-openapi.yml
- filename: capgo-app-devices-api-openapi.yml
  format: yaml
  label: Capgo Devices API
  slug: capgo-app-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-devices-api-openapi.yml
- filename: capgo-app-members-api-openapi.yml
  format: yaml
  label: Capgo Members API
  slug: capgo-app-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-members-api-openapi.yml
- filename: capgo-app-organizations-api-openapi.yml
  format: yaml
  label: Capgo Organizations API
  slug: capgo-app-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-organizations-api-openapi.yml
- filename: capgo-app-statistics-api-openapi.yml
  format: yaml
  label: Capgo Statistics API
  slug: capgo-app-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-statistics-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: capgo.app
  spf: true
hosts:
- cert_expires: Jan 31 05:20:34 2027 GMT
  host: capgo.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capgo App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capgo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Capgo
provider_slug: capgo-app
slug: capgo-app-domain-security
source_filename: capgo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capgo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 05:20:34 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: capgo.app\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/capgo-app/security/capgo-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Mobile
- Development
- Capacitor
---
