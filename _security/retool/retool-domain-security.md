---
api_specs:
- filename: retool-management-api-openapi.yml
  format: yaml
  label: Retool Management API
  slug: retool-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/openapi/retool-management-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: retool.com
  spf: true
hosts:
- cert_expires: Sep 26 05:48:02 2026 GMT
  host: retool.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 20:14:58 2026 GMT
  host: docs.retool.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 09:08:17 2026 GMT
  host: api.retool.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Retool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Retool, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Retool
provider_slug: retool
slug: retool-domain-security
source_filename: retool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: retool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:48:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.retool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.retool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 09:08:17 2026 GMT\n  hsts: null\ndomains:\n- domain: retool.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/security/retool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Admin Panel
- Dashboard
- Internal Tools
- Low Code
- No Code
---
