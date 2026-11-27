---
api_specs:
- filename: himalayas-app-api-openapi.json
  format: json
  label: Himalayas Remote Jobs API API
  slug: himalayas-remote-jobs-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/himalayas-app/openapi/_original/himalayas-app-api-openapi.json
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
  domain: himalayas.app
  spf: true
hosts:
- cert_expires: Feb  6 09:36:14 2027 GMT
  host: himalayas.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Himalayas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Himalayas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Himalayas
provider_slug: himalayas-app
slug: himalayas-app-domain-security
source_filename: himalayas-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: himalayas.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 09:36:14 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: himalayas.app\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/himalayas-app/security/himalayas-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Remote Jobs
- AI Tools
- Job Search
- Careers
- Technology
---
