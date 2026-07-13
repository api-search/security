---
api_specs:
- filename: kickbox-openapi.yml
  format: yaml
  label: Kickbox Email Verification API
  slug: verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kickbox.com
  spf: true
hosts:
- cert_expires: Sep 13 21:42:56 2026 GMT
  host: kickbox.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:04:43 2026 GMT
  host: docs.kickbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.kickbox.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kickbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kickbox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kickbox
provider_slug: kickbox
slug: kickbox-domain-security
source_filename: kickbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kickbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:42:56 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.kickbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:04:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kickbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: kickbox.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/security/kickbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Verification
- Email Validation
- Deliverability
- Data Quality
- Email
---
