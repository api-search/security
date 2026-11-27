---
api_specs:
- filename: erzycall-com-openapi-generated.yml
  format: yaml
  label: ErzyCall API
  slug: erzycall-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/erzycall-com/openapi/_ae-authored/erzycall-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: erzycall.com
  spf: true
hosts:
- cert_expires: Jan 23 16:23:15 2027 GMT
  host: erzycall.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ErzyCall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ErzyCall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ErzyCall
provider_slug: erzycall-com
slug: erzycall-com-domain-security
source_filename: erzycall-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: erzycall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 16:23:15 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: erzycall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/erzycall-com/security/erzycall-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Call
- Virtual Receptionist
- Inbound Calls
- Outbound Calls
- WhatsApp
- Appointment Scheduling
- CRM Integration
- Call Analytics
---
