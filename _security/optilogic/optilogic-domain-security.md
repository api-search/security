---
api_specs:
- filename: optilogic-rest-api-openapi.json
  format: json
  label: Optilogic REST API
  slug: optilogic-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/openapi/optilogic-rest-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: optilogic.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: optilogic.app
  spf: true
hosts:
- cert_expires: Nov  4 20:40:17 2026 GMT
  host: optilogic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 02:50:15 2026 GMT
  host: api-docs.optilogic.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 01:05:48 2026 GMT
  host: api.optilogic.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optilogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optilogic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Optilogic
provider_slug: optilogic
slug: optilogic-domain-security
source_filename: optilogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optilogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 20:40:17 2026 GMT\n  hsts: false\n- host: api-docs.optilogic.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 02:50:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.optilogic.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:05:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: optilogic.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: optilogic.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optilogic/refs/heads/main/security/optilogic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Supply Chain
- Supply Chain Design
- Network Optimization
- Simulation
- Optimization
- Logistics
- Analytics
- Artificial Intelligence
- Jobs
- Cloud
---
