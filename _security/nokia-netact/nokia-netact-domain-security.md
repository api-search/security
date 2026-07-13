---
api_specs:
- filename: nokia-netact-nbi-openapi.yml
  format: yaml
  label: Nokia NetAct / Ericsson OSS API
  slug: nokia-netact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-netact/refs/heads/main/openapi/nokia-netact-nbi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nokia.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.nokia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nokia Netact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nokia NetAct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nokia NetAct
provider_slug: nokia-netact
slug: nokia-netact-domain-security
source_filename: nokia-netact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nokia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nokia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nokia-netact/refs/heads/main/security/nokia-netact-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Network Management
- OSS
- SNMP
- Telecom
---
