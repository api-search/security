---
api_specs:
- filename: ixon-openapi.json
  format: json
  label: IXON Cloud API
  slug: ixon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ixon/refs/heads/main/openapi/ixon-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ixon.cloud
  spf: true
hosts:
- cert_expires: Aug 13 21:48:36 2026 GMT
  host: www.ixon.cloud
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:44:51 2026 GMT
  host: developer.ixon.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 20:04:28 2026 GMT
  host: portal.ixon.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ixon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IXON, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IXON
provider_slug: ixon
slug: ixon-domain-security
source_filename: ixon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ixon.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 21:48:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.ixon.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:44:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.ixon.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 20:04:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ixon.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ixon/refs/heads/main/security/ixon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IIoT
- Industrial IoT
- Machine Connectivity
- Remote Access
---
