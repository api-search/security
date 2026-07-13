---
api_specs:
- filename: opnsense-openapi.yml
  format: yaml
  label: OPNsense Core REST API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opnsense/refs/heads/main/openapi/opnsense-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opnsense.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: opnsense.local
  spf: false
hosts:
- cert_expires: Oct  4 16:51:48 2026 GMT
  host: opnsense.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 03:51:30 2026 GMT
  host: docs.opnsense.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: opnsense.local
  https: false
kind: domain-security
layout: security
method: probed
name: Opnsense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OPNsense, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OPNsense
provider_slug: opnsense
slug: opnsense-domain-security
source_filename: opnsense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opnsense.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:51:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.opnsense.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 03:51:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opnsense.local\n  https: false\ndomains:\n- domain: opnsense.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: opnsense.local\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opnsense/refs/heads/main/security/opnsense-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Firewall
- Networking
- Security
- VPN
- Routing
- Open Source
---
