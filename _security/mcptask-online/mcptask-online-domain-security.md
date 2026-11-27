---
api_specs:
- filename: mcptask-online-openapi-generated.yml
  format: yaml
  label: WorkVector s.r.o. API
  slug: mcptask-online-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcptask-online/openapi/_ae-authored/mcptask-online-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mcptask.online
  spf: true
hosts:
- cert_expires: Jan 15 22:17:37 2027 GMT
  host: mcptask.online
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: WorkVector s.r.o. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorkVector s.r.o., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WorkVector s.r.o.
provider_slug: mcptask-online
slug: mcptask-online-domain-security
source_filename: mcptask-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcptask.online\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 22:17:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcptask.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mcptask-online/security/mcptask-online-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Artificial Intelligence
- Developer Tools
- Automation
- Czech Republic
- Software-as-a-Service
---
