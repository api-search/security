---
api_specs:
- filename: senseon-openapi-generated.yml
  format: yaml
  label: SenseOn API
  slug: senseon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/senseon/openapi/_ae-authored/senseon-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: senseon.io
  spf: true
hosts:
- cert_expires: Dec  2 01:58:22 2026 GMT
  host: www.senseon.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Senseon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SenseOn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SenseOn
provider_slug: senseon
slug: senseon-domain-security
source_filename: senseon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.senseon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 01:58:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: senseon.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/senseon/security/senseon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- AI
- Platform
- Incident-Response
---
