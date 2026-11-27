---
api_specs:
- filename: tellescope-openapi-generated.yml
  format: yaml
  label: Tellescope API
  slug: tellescope-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tellescope/openapi/_ae-authored/tellescope-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tellescope.com
  spf: true
hosts:
- cert_expires: Jan 17 19:44:48 2027 GMT
  host: tellescope.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tellescope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tellescope, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tellescope
provider_slug: tellescope
slug: tellescope-domain-security
source_filename: tellescope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tellescope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:44:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tellescope.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tellescope/security/tellescope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Health
- Patient Intake
- EHR Integration
- Telehealth
- Workflow Automation
- Healthcare CRM
---
