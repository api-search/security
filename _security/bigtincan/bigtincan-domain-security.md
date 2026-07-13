---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Bigtincan Hub API
  slug: bigtincan-hub-api
  spec_type: OpenAPI
  url: https://pubapi.bigtincan.com/doc/interactive/
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@bigtincan.com"
  - 0 issue "amazon.com"
  - 0 issue "certs.godaddy.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bigtincan.com
  spf: true
hosts:
- cert_expires: Oct  2 03:11:54 2026 GMT
  host: www.bigtincan.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:42:21 2026 GMT
  host: help.bigtincan.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: pubapi.bigtincan.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bigtincan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigtincan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bigtincan
provider_slug: bigtincan
slug: bigtincan-domain-security
source_filename: bigtincan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bigtincan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:11:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.bigtincan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:42:21 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: pubapi.bigtincan.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bigtincan.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@bigtincan.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certs.godaddy.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigtincan/refs/heads/main/security/bigtincan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Enablement
- Content Management
- Training
- Coaching
- Buyer Engagement
- Analytics
- CRM Integration
- Digital Sales Rooms
---
