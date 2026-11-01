---
api_specs:
- filename: lobster-world-channels-api-openapi.yml
  format: yaml
  label: Lobster Data GmbH Channels API
  slug: lobster-world-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lobster-world/openapi/lobster-world-channels-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lobster-world.com
  spf: true
hosts:
- cert_expires: Dec 15 08:50:45 2026 GMT
  host: lobster-world.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lobster World Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lobster Data GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lobster Data GmbH
provider_slug: lobster-world
slug: lobster-world-domain-security
source_filename: lobster-world-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lobster-world.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 08:50:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lobster-world.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lobster-world/security/lobster-world-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Analytics
- IoT
- Real-Time
---
