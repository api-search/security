---
api_specs:
- filename: meteoblue-openapi-generated.yml
  format: yaml
  label: Meteoblue API
  slug: meteoblue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meteoblue/openapi/_ae-authored/meteoblue-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meteoblue.com
  spf: true
hosts:
- cert_expires: Dec  2 16:08:08 2026 GMT
  host: meteoblue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meteoblue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meteoblue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Meteoblue
provider_slug: meteoblue
slug: meteoblue-domain-security
source_filename: meteoblue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meteoblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 16:08:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: meteoblue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/meteoblue/security/meteoblue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Weather
- Climate
- Data
- API
- Forecast
---
