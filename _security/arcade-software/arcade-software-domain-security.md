---
api_specs:
- filename: arcade-software-openapi-generated.yml
  format: yaml
  label: Arcade API
  slug: arcade-software-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcade-software/openapi/_ae-authored/arcade-software-openapi-generated.yml
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
  domain: arcade.software
  spf: true
hosts:
- cert_expires: Feb 10 05:44:11 2027 GMT
  host: arcade.software
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arcade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arcade
provider_slug: arcade-software
slug: arcade-software-domain-security
source_filename: arcade-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcade.software\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 05:44:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arcade.software\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/arcade-software/security/arcade-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Video
- Marketing
- Automation
- Platform
---
