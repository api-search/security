---
api_specs:
- filename: introduction
  format: yaml
  label: Plane REST API
  slug: plane-rest-api
  spec_type: OpenAPI
  url: https://developers.plane.so/api-reference/introduction
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plane.so
  spf: true
hosts:
- cert_expires: Oct  8 05:33:03 2026 GMT
  host: plane.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 03:55:34 2026 GMT
  host: developers.plane.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 09:46:37 2026 GMT
  host: api.plane.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plane, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plane
provider_slug: plane
slug: plane-domain-security
source_filename: plane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plane.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.plane.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:55:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.plane.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:46:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plane.so\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plane/refs/heads/main/security/plane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Project Management
- Issues
- Cycles
- Modules
- Pages
- Analytics
- Workspace
- Open Source
- Self-Hosted
- AI
---
