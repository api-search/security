---
api_specs:
- filename: eat-reservations-api-openapi.yml
  format: yaml
  label: Eat Reservations API
  slug: eat-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eat/openapi/eat-reservations-api-openapi.yml
- filename: eat-openapi-generated.yml
  format: yaml
  label: Eat API
  slug: eat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eat/openapi/_ae-authored/eat-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: eatapp.co
  spf: true
hosts:
- cert_expires: Dec 18 17:53:09 2026 GMT
  host: eatapp.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Eat
provider_slug: eat
slug: eat-domain-security
source_filename: eat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eatapp.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 17:53:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eatapp.co\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eat/security/eat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Restaurant
- Reservation
- SaaS
- Hospitality
---
