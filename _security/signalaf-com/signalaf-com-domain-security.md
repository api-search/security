---
api_specs:
- filename: signalaf-com-hall-api-openapi.yml
  format: yaml
  label: signalaf-com Hall API
  slug: signalaf-com-hall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalaf-com/openapi/signalaf-com-hall-api-openapi.yml
- filename: signalaf-com-leaderboard-api-openapi.yml
  format: yaml
  label: signalaf-com Leaderboard API
  slug: signalaf-com-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalaf-com/openapi/signalaf-com-leaderboard-api-openapi.yml
- filename: signalaf-com-metrics-api-openapi.yml
  format: yaml
  label: signalaf-com Metrics API
  slug: signalaf-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalaf-com/openapi/signalaf-com-metrics-api-openapi.yml
- filename: signalaf-com-operators-api-openapi.yml
  format: yaml
  label: signalaf-com Operators API
  slug: signalaf-com-operators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signalaf-com/openapi/signalaf-com-operators-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signalaf.com
  spf: true
hosts:
- cert_expires: Jan 17 21:10:09 2027 GMT
  host: signalaf.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Signalaf Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for signalaf-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: signalaf-com
provider_slug: signalaf-com
slug: signalaf-com-domain-security
source_filename: signalaf-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signalaf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 21:10:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: signalaf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/signalaf-com/security/signalaf-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Analytics
- Leaderboard
- OpenAPI
- PublicAPI
---
