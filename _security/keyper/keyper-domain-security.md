---
api_specs:
- filename: keyper-access-openapi.yml
  format: yaml
  label: keyper Access API
  slug: keyper-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keyper/refs/heads/main/openapi/keyper-access-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keyper.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keyper.io
  spf: true
hosts:
- cert_expires: Sep 14 15:16:03 2026 GMT
  host: www.keyper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 14:54:44 2026 GMT
  host: developers.keyper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.keyper.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Keyper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keyper, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Keyper
provider_slug: keyper
slug: keyper-domain-security
source_filename: keyper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keyper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:16:03 2026 GMT\n  hsts: false\n- host: developers.keyper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:54:44 2026 GMT\n  hsts: false\n- host: api.keyper.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: keyper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: keyper.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyper/refs/heads/main/security/keyper-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ticketing
- Access Control
- Events
- Developer Platform
- SDK
- Sports
- Arts and Culture
- Austria
---
