---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gooseinsurance.com
  spf: true
hosts:
- cert_expires: Oct 22 23:06:56 2026 GMT
  host: www.gooseinsurance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:31:27 2026 GMT
  host: api.gooseinsurance.com
  hsts: false
  https: true
  note: 'Private Heroku-fronted mobile-app backend (server: Heroku, heroku-nel reporting headers). Answers HTTP/2 404 at every probed path; no HSTS header is returned. Not a documented product API.'
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:40:22 2026 GMT
  host: support.gooseinsurance.com
  hsts: true
  hsts_max_age: 259200
  https: true
  note: Zendesk consumer help center; blocks non-browser agents (403).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goose Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goose Insurance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Goose Insurance
provider_slug: goose-insurance
slug: goose-insurance-domain-security
source_filename: goose-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gooseinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:06:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gooseinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:31:27 2026 GMT\n  hsts: false\n  note: >-\n    Private Heroku-fronted mobile-app backend (server: Heroku, heroku-nel\n    reporting headers). Answers HTTP/2 404 at every probed path; no HSTS header\n    is returned. Not a documented product API.\n- host: support.gooseinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:40:22 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  note: Zendesk consumer help center; blocks non-browser agents (403).\ndomains:\n- domain: gooseinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goose-insurance/refs/heads/main/security/goose-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Insurtech
- Life Insurance
- Travel Insurance
- Health Insurance
- Broker
- Digital Distribution
- Managing General Agent
- Mobile
---
