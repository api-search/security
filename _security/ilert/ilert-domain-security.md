---
api_specs:
- filename: ilert-ilert-rest-api-openapi.yml
  format: yaml
  label: ilert REST API
  slug: ilert-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ilert/refs/heads/main/openapi/ilert-ilert-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ilert.com
  spf: true
hosts:
- cert_expires: Aug 16 07:51:20 2026 GMT
  host: www.ilert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 21:42:51 2026 GMT
  host: docs.ilert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: api.ilert.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ilert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ilert, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ilert
provider_slug: ilert
slug: ilert-domain-security
source_filename: ilert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ilert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:51:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ilert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:42:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ilert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ilert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ilert/refs/heads/main/security/ilert-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Incident Management
- On-Call Alerting
- Alert Routing
- Escalation Policies
- On-Call Schedules
- Status Pages
- Heartbeat Monitoring
- Event Management
- DevOps
- SRE
- IT Operations
---
