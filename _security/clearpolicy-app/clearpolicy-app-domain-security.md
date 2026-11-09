---
api_specs:
- filename: clearpolicy-app-api-openapi.json
  format: json
  label: ClearPolicy API API
  slug: clearpolicy-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearpolicy-app/openapi/_original/clearpolicy-app-api-openapi.json
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
  dmarc_policy: reject
  dnssec: false
  domain: clearpolicy.app
  spf: true
hosts:
- cert_expires: Dec 22 18:13:56 2026 GMT
  host: clearpolicy.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clearpolicy App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearPolicy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClearPolicy
provider_slug: clearpolicy-app
slug: clearpolicy-app-domain-security
source_filename: clearpolicy-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearpolicy.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 18:13:56 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: clearpolicy.app\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/clearpolicy-app/security/clearpolicy-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Policy
- E-Signature
- Software-as-a-Service
- Small Business
- Non-Profit
---
