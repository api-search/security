---
api_specs:
- filename: ko-fi-asyncapi.yml
  format: yaml
  label: Ko-fi Webhook
  slug: ko-fi-webhook
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ko-fi/refs/heads/main/asyncapi/ko-fi-asyncapi.yml
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
  dmarc_policy: reject
  dnssec: false
  domain: ko-fi.com
  spf: true
hosts:
- cert_expires: Sep 28 20:42:18 2026 GMT
  host: ko-fi.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 12 23:40:50 2026 GMT
  host: help.ko-fi.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ko Fi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ko-fi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ko-fi
provider_slug: ko-fi
slug: ko-fi-domain-security
source_filename: ko-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ko-fi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 20:42:18 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: help.ko-fi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:40:50 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: ko-fi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ko-fi/refs/heads/main/security/ko-fi-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Creator Economy
- Donations
- Tips
- Memberships
- Shop
- Payments
- Webhooks
- Creator Monetization
---
