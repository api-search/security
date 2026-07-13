---
api_specs:
- filename: hightouch-openapi.yml
  format: yaml
  label: Hightouch API
  slug: hightouch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hightouch.com
  spf: true
hosts:
- cert_expires: Aug 13 01:56:29 2026 GMT
  host: hightouch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api.hightouch.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hightouch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hightouch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hightouch
provider_slug: hightouch
slug: hightouch-domain-security
source_filename: hightouch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hightouch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:56:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hightouch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hightouch.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/security/hightouch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CDP
- Data Activation
- Reverse ETL
- Audience Management
- Unified API
- Marketing
---
