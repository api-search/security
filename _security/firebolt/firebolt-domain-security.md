---
api_specs:
- filename: firebolt-openapi.yml
  format: yaml
  label: Firebolt REST API
  slug: firebolt-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firebolt/refs/heads/main/openapi/firebolt-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:devops@firebolt.io"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firebolt.io
  spf: true
hosts:
- cert_expires: Sep 17 07:00:32 2026 GMT
  host: www.firebolt.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 16:39:36 2026 GMT
  host: docs.firebolt.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.app.firebolt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firebolt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firebolt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Firebolt
provider_slug: firebolt
slug: firebolt-domain-security
source_filename: firebolt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firebolt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 07:00:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.firebolt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:39:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.app.firebolt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: firebolt.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:devops@firebolt.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firebolt/refs/heads/main/security/firebolt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Warehouse
- Cloud
- SQL
- Analytics
---
