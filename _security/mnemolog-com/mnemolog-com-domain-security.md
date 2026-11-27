---
api_specs:
- filename: mnemolog-com-openapi-generated.yml
  format: yaml
  label: Mnemolog API
  slug: mnemolog-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemolog-com/openapi/_ae-authored/mnemolog-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: true
  domain: mnemolog.com
  spf: false
hosts:
- cert_expires: Dec 26 17:31:11 2026 GMT
  host: mnemolog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mnemolog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mnemolog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Mnemolog
provider_slug: mnemolog-com
slug: mnemolog-com-domain-security
source_filename: mnemolog-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mnemolog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 17:31:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mnemolog.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mnemolog-com/security/mnemolog-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Artificial Intelligence
- Memory
- Privacy
- Productivity
- Platform
---
