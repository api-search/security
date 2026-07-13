---
api_specs:
- filename: port-openapi.yml
  format: yaml
  label: Port API
  slug: port
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/openapi/port-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: port.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getport.io
  spf: true
hosts:
- cert_expires: Sep 19 15:41:46 2026 GMT
  host: www.port.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: docs.getport.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.getport.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Port Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Port, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Port
provider_slug: port
slug: port-domain-security
source_filename: port-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.port.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:41:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getport.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\n- host: api.getport.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: port.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getport.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/port/refs/heads/main/security/port-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automations
- Developer Portals
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Software Catalog
---
