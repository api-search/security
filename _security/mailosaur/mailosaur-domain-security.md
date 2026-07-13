---
api_specs:
- filename: mailosaur-mailosaur-api-openapi.yml
  format: yaml
  label: Mailosaur API
  slug: mailosaur-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-mailosaur-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailosaur.com
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: mailosaur.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailosaur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailosaur, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mailosaur
provider_slug: mailosaur
slug: mailosaur-domain-security
source_filename: mailosaur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailosaur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailosaur.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/security/mailosaur-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Testing
- SMS Testing
- Developer Tools
- QA Automation
- CI/CD
- SMTP
- TOTP
- Deliverability
---
