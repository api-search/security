---
api_specs:
- filename: got-its-openapi-original.yml
  format: yaml
  label: Reelables API
  slug: reelables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/openapi/got-its-openapi-original.yml
- filename: got-its-gateway-openapi-original.yml
  format: yaml
  label: Reelables Gateway API
  slug: reelables-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/openapi/got-its-gateway-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue " letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reelables.com
  spf: true
hosts:
- cert_expires: Sep  9 15:02:58 2026 GMT
  host: reelables.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 06:01:50 2026 GMT
  host: docs.reelables.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.reelables.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Got Its Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reelables, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reelables
provider_slug: got-its
slug: got-its-domain-security
source_filename: got-its-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reelables.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 15:02:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.reelables.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 06:01:50 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.reelables.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reelables.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/got-its/refs/heads/main/security/got-its-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Supply Chain
- Logistics
- Asset Tracking
- IoT
- Smart Labels
- Bluetooth
- Cellular
- Track and Trace
- Location
---
