---
api_specs:
- filename: divinci-app-api-openapi.yml
  format: yaml
  label: Divinci AI API API
  slug: divinci-ai-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/divinci-app/openapi/_original/divinci-app-api-openapi.yml
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
  dmarc_policy: none
  dnssec: true
  domain: divinci.app
  spf: true
hosts:
- cert_expires: Feb  3 04:14:33 2027 GMT
  host: divinci.app
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Divinci App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Divinci, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Divinci
provider_slug: divinci-app
slug: divinci-app-domain-security
source_filename: divinci-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: divinci.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 04:14:33 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: divinci.app\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/divinci-app/security/divinci-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Website Integration
- Conversational AI
- No-Code
- Customer Service
- phone integration
---
