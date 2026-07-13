---
api_specs:
- filename: nimble-openapi.yml
  format: yaml
  label: Nimble REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:admin@nimble.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nimble.com
  spf: true
hosts:
- cert_expires: Sep 22 23:18:47 2026 GMT
  host: www.nimble.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:18:47 2026 GMT
  host: api.nimble.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:18:47 2026 GMT
  host: app.nimble.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nimble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nimble, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nimble
provider_slug: nimble
slug: nimble-domain-security
source_filename: nimble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: app.nimble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: nimble.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:admin@nimble.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/security/nimble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Sales
- Contact Management
- Relationship Management
- Marketing Automation
- Pipeline Management
---
