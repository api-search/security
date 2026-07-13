---
api_specs:
- filename: bigpanda-openapi.yml
  format: yaml
  label: BigPanda
  slug: bigpanda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/openapi/bigpanda-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bigpanda.io
  spf: true
hosts:
- cert_expires: Aug 31 03:49:07 2026 GMT
  host: docs.bigpanda.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 20:40:41 2026 GMT
  host: api.bigpanda.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bigpanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BigPanda, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BigPanda
provider_slug: bigpanda
slug: bigpanda-domain-security
source_filename: bigpanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.bigpanda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:49:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bigpanda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:40:41 2026 GMT\n  hsts: null\ndomains:\n- domain: bigpanda.io\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/security/bigpanda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Incidents
- Monitoring
- Platform
---
