---
api_specs:
- filename: routeros-rest-api-openapi.yml
  format: yaml
  label: RouterOS REST API
  slug: routeros-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mikrotik.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: mikrotik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 26 04:09:31 2026 GMT
  host: help.mikrotik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Routeros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RouterOS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RouterOS
provider_slug: routeros
slug: routeros-domain-security
source_filename: routeros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mikrotik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.mikrotik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 04:09:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mikrotik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/security/routeros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Networking
- Routers
- Network Management
- Firewall
- MikroTik
---
