---
api_specs:
- filename: fynqo-app-well-known-openapi.json
  format: json
  label: Fynqo Public API .well-known API
  slug: fynqo-public-api-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fynqo-app/openapi/_original/fynqo-app-well-known-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:johanvd75@gmail.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fynqo.app
  spf: true
hosts:
- cert_expires: Jan 25 06:45:10 2027 GMT
  host: fynqo.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fynqo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fynqo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fynqo
provider_slug: fynqo-app
slug: fynqo-app-domain-security
source_filename: fynqo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fynqo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 06:45:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fynqo.app\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:johanvd75@gmail.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fynqo-app/security/fynqo-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Document Management
- Task Management
- Software-as-a-Service
- Productivity
- Company
---
