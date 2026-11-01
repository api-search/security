---
api_specs:
- filename: tessie-driver-management-api-openapi.yml
  format: yaml
  label: Tessie Driver Management API
  slug: tessie-driver-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-driver-management-api-openapi.yml
- filename: tessie-telemetry-configuration-api-openapi.yml
  format: yaml
  label: Tessie Telemetry Configuration API
  slug: tessie-telemetry-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-telemetry-configuration-api-openapi.yml
- filename: tessie-vehicle-commands-api-openapi.yml
  format: yaml
  label: Tessie Vehicle Commands API
  slug: tessie-vehicle-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-vehicle-commands-api-openapi.yml
- filename: tessie-vehicle-data-api-openapi.yml
  format: yaml
  label: Tessie Vehicle Data API
  slug: tessie-vehicle-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-vehicle-data-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tessie.com
  spf: true
hosts:
- cert_expires: Dec 19 16:47:17 2026 GMT
  host: tessie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tessie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tessie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tessie
provider_slug: tessie
slug: tessie-domain-security
source_filename: tessie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tessie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 16:47:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tessie.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tessie/security/tessie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Tesla
- Fleet Management
- Automotive
- APIs
---
