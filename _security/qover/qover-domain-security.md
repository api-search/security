---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Qover Embedded Insurance API
  slug: qover-embedded-insurance-api
  spec_type: Postman
  url: https://docs.qover.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qover.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qover.io
  spf: false
hosts:
- cert_expires: Oct  2 12:12:07 2026 GMT
  host: docs.qover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 21:30:59 2026 GMT
  host: api.sbx.qover.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qover, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qover
provider_slug: qover
slug: qover-domain-security
source_filename: qover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.qover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:12:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sbx.qover.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:30:59 2026 GMT\n  hsts: null\ndomains:\n- domain: qover.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: qover.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qover/refs/heads/main/security/qover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Insurance
- Embedded Insurance
- Claims
- Policy
- API
- Fintech
- Belgium
---
