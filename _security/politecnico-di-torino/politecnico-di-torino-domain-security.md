---
api_specs:
- filename: politecnico-di-torino-students-api.yaml
  format: yaml
  label: PoliTO REST API (api-spec)
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/openapi/politecnico-di-torino-students-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: polito.it
  spf: true
hosts:
- cert_expires: Nov  6 14:21:43 2026 GMT
  host: www.polito.it
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 01:56:53 2026 GMT
  host: app.didattica.polito.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Politecnico Di Torino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Politecnico di Torino, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Politecnico di Torino
provider_slug: politecnico-di-torino
slug: politecnico-di-torino-domain-security
source_filename: politecnico-di-torino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polito.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 14:21:43 2026 GMT\n  hsts: false\n- host: app.didattica.polito.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 01:56:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: polito.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/politecnico-di-torino/refs/heads/main/security/politecnico-di-torino-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Italy
- Open Data
- Mobile
- OpenAPI
---
