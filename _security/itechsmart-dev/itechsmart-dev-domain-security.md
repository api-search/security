---
api_specs:
- filename: itechsmart-dev-openapi-generated.yml
  format: yaml
  label: iTechSmart API
  slug: itechsmart-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itechsmart-dev/openapi/_ae-authored/itechsmart-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: itechsmart.dev
  spf: true
hosts:
- cert_expires: Dec 17 22:09:02 2026 GMT
  host: itechsmart.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: iTechSmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iTechSmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iTechSmart
provider_slug: itechsmart-dev
slug: itechsmart-dev-domain-security
source_filename: itechsmart-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: itechsmart.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 22:09:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: itechsmart.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/itechsmart-dev/security/itechsmart-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AutonomousOps
- Artificial Intelligence
- Monitoring
- Automation
---
