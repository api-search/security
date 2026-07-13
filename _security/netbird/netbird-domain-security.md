---
api_specs:
- filename: netbird-openapi.yml
  format: yaml
  label: NetBird
  slug: netbird
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netbird/refs/heads/main/openapi/netbird-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netbird.io
  spf: true
hosts:
- cert_expires: Sep  6 11:09:25 2026 GMT
  host: netbird.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 11:09:25 2026 GMT
  host: docs.netbird.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 03:57:34 2026 GMT
  host: api.netbird.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netbird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetBird, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NetBird
provider_slug: netbird
slug: netbird-domain-security
source_filename: netbird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netbird.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 11:09:25 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.netbird.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 11:09:25 2026 GMT\n  hsts: false\n- host: api.netbird.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:57:34 2026 GMT\n  hsts: null\ndomains:\n- domain: netbird.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netbird/refs/heads/main/security/netbird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Networking
- VPN
- Zero Trust
- Open Source
- WireGuard
- Security
---
