---
api_specs:
- filename: teslalogger-openapi-generated.yml
  format: yaml
  label: TeslaLogger (self-hosted) API
  slug: teslalogger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslalogger/openapi/_ae-authored/teslalogger-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teslalogger.de
  spf: true
hosts:
- cert_expires: Nov 27 16:28:51 2026 GMT
  host: teslalogger.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Teslalogger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeslaLogger (self-hosted), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TeslaLogger (self-hosted)
provider_slug: teslalogger
slug: teslalogger-domain-security
source_filename: teslalogger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teslalogger.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 16:28:51 2026 GMT\n  hsts: false\ndomains:\n- domain: teslalogger.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/teslalogger/security/teslalogger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- DataLogging
- OpenSource
- Tesla
---
