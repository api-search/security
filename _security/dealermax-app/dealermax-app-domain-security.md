---
api_specs:
- filename: dealermax-app-dealerpublicapi-api-openapi.yml
  format: yaml
  label: DealerMAX Dealer Public API
  slug: dealermax-app-dealerpublicapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealermax-app/openapi/dealermax-app-dealerpublicapi-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@dealermax.app"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dealermax.app
  spf: true
hosts:
- cert_expires: Jan  4 19:07:40 2027 GMT
  host: dealermax.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DealerMAX Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DealerMAX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DealerMAX
provider_slug: dealermax-app
slug: dealermax-app-domain-security
source_filename: dealermax-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealermax.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 19:07:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dealermax.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@dealermax.app\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dealermax-app/security/dealermax-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dealer Identity
- AI Visibility
- CRM
---
