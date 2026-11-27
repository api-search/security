---
api_specs:
- filename: myzone-accounts-api-openapi.yml
  format: yaml
  label: Myzone Accounts API
  slug: myzone-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-accounts-api-openapi.yml
- filename: myzone-biometrics-api-openapi.yml
  format: yaml
  label: Myzone Biometrics API
  slug: myzone-biometrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-biometrics-api-openapi.yml
- filename: myzone-challenges-api-openapi.yml
  format: yaml
  label: Myzone Challenges API
  slug: myzone-challenges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-challenges-api-openapi.yml
- filename: myzone-classes-and-booking-api-openapi.yml
  format: yaml
  label: Myzone Classes And Booking API
  slug: myzone-classes-and-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-classes-and-booking-api-openapi.yml
- filename: myzone-facilities-api-openapi.yml
  format: yaml
  label: Myzone Facilities API
  slug: myzone-facilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-facilities-api-openapi.yml
- filename: myzone-groups-api-openapi.yml
  format: yaml
  label: Myzone Groups API
  slug: myzone-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-groups-api-openapi.yml
- filename: myzone-moves-api-openapi.yml
  format: yaml
  label: Myzone Moves API
  slug: myzone-moves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-moves-api-openapi.yml
- filename: myzone-reports-api-openapi.yml
  format: yaml
  label: Myzone Reports API
  slug: myzone-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-reports-api-openapi.yml
- filename: myzone-webhooks-api-openapi.yml
  format: yaml
  label: Myzone Webhooks API
  slug: myzone-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myzone/openapi/myzone-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myzone.org
  spf: true
hosts:
- cert_expires: Jan  3 05:31:45 2027 GMT
  host: myzone.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Myzone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Myzone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Myzone
provider_slug: myzone
slug: myzone-domain-security
source_filename: myzone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myzone.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 05:31:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: myzone.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/myzone/security/myzone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- MotivationTechnology
- Wearables
- Gym Management
- Software-as-a-Service
- Company
---
