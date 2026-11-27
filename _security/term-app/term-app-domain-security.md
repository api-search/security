---
api_specs:
- filename: term-app-api-openapi.json
  format: json
  label: TERM onboarding REST API API
  slug: term-onboarding-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/term-app/openapi/_original/term-app-api-openapi.json
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
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: term.app
  spf: true
hosts:
- cert_expires: Feb  7 22:35:02 2027 GMT
  host: term.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TERM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TERM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TERM
provider_slug: term-app
slug: term-app-domain-security
source_filename: term-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: term.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 22:35:02 2027 GMT\n  hsts: false\ndomains:\n- domain: term.app\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/term-app/security/term-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Forum
- OpenAPI
- Community
- Deterministic
---
