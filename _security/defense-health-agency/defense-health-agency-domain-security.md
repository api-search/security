---
api_specs:
- filename: defense-health-agency-openapi.yml
  format: yaml
  label: MHS Genesis SMART on FHIR API
  slug: mhs-genesis-smart-on-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/defense-health-agency/refs/heads/main/openapi/defense-health-agency-openapi.yml
description: ''
domains:
- caa:
  - 128 issue "digicert.com"
  - 128 issue "entrust.net"
  - 128 issue "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: health.mil
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.health.mil
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: health.mil
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Defense Health Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Health Agency, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Health Agency
provider_slug: defense-health-agency
slug: defense-health-agency-domain-security
source_filename: defense-health-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.health.mil\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: health.mil\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: health.mil\n  dnssec: true\n  caa:\n  - 128 issue \"digicert.com\"\n  - 128 issue \"entrust.net\"\n  - 128 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-health-agency/refs/heads/main/security/defense-health-agency-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Defense
- Department of Defense
- Health
- Military Health System
- MHS Genesis
- FHIR
- Health IT
---
