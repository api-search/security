---
api_specs:
- filename: elmah-io-v3-openapi.json
  format: json
  label: elmah.io API V3 API
  slug: elmah-io-api-v3-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elmah-io/openapi/_original/elmah-io-v3-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: elmah.io
  spf: true
hosts:
- cert_expires: Feb  3 19:23:01 2027 GMT
  host: elmah.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: elmah.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for elmah.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: elmah.io
provider_slug: elmah-io
slug: elmah-io-domain-security
source_filename: elmah-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elmah.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 19:23:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elmah.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/elmah-io/security/elmah-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Logging
- Monitoring
- .NET
- Error Tracking
- Cloud
---
