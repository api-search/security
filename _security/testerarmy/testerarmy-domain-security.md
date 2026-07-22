---
api_specs:
- filename: testerarmy-openapi-original.json
  format: json
  label: TesterArmy API
  slug: testerarmy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testerarmy/refs/heads/main/openapi/testerarmy-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tester.army
  spf: true
hosts:
- cert_expires: Sep 13 14:11:15 2026 GMT
  host: tester.army
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Testerarmy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Testerarmy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Testerarmy
provider_slug: testerarmy
slug: testerarmy-domain-security
source_filename: testerarmy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tester.army\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:11:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tester.army\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testerarmy/refs/heads/main/security/testerarmy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- QA
- Software Testing
- Browser Automation
- AI Agents
- Developer Tools
- CI/CD
- End-to-End Testing
- Mobile Testing
---
